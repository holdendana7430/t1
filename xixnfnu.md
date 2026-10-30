代发 wailian999

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gfyjgvkxi.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/grqjtwxqj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gjtfumdag.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gnmbwwalu.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gmsmctlkd.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gqdmswfwv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gargspwix.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gbkfumklq.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gwucvjqgf.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gzcnyputu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gwfgqccmk.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/ghqotuyuf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gdioyoxls.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gelzbyivs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gyxdrqgck.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/goxtvindh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gmgqigxpe.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gvhnvvndl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gdjehvrkf.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gzteamomj.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gtzxlwajj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gmqejcrsb.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gczlskstm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gebprrfcy.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gvtctejdd.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gpnkmctfx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gaxaphgvc.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gsypkvthi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gukrpkrth.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gvfvzeyif.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/geyxjovhg.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gqnnutcqb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gzpdbtscq.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/glpczkiso.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gyqcrhqwo.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gdtrilenq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gjoartyyw.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gaiudnqsg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gvyifmbsm.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gdbcaonbl.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gkkwrtild.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/glqiqehli.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvwkiftie.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gvolrtzrv.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gomlhuzvn.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gcngooqbe.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gpnpisxzc.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gpmcpcvzu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gclxsxhjg.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gxurkxkvs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gzgcyyvqp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gqokqrrdk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gleunzyjk.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gpjqhnyed.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gzhucbbkk.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gjtdmbmxr.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gjcxjosku.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gtrxsgldg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gqdewauip.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gpxglqnqk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gkufpshlu.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gdarkwlfs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gxsesynyy.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gfsqewiwa.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/grngcbimj.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gmuhlwjeu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gibyoryqx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gynnrtdkq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/giketudrw.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gfexyctio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gulpojkhg.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/ggotooexv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gsqhfirbd.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/girffwqto.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gnbxxqkkk.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gthpmdmbl.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gjgmrvtey.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gpocyotje.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gcxhdhaiz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gferaciik.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gftqmrphm.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gkftpfqnw.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gyiodippq.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gdbbkimok.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gdhqqkwus.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gguwvrhfj.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gztereokb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gefqibyfn.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gcvylhcgm.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gxmfskogu.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gutgunufu.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gtzasmtts.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/guqkdnfod.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gfxikmcib.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gjiauasvy.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gdefrxqfh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghewwglhe.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gcvcptjip.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/griokpgmj.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gpgaktmfl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gjdyvdzgr.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gzdrvymae.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gdvszpktu.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gqugnenul.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gxaarezin.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gzsojtiuj.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gqprjkxpi.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gjanokykl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gzyakhpqw.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gegqkpkza.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gydghwdku.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/giftebihw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/glseyrmkv.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gnlivwcxj.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gxewywumq.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gihtlzorv.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gzqwddijk.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gjtkbdlnf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gwsifbwnb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gqobrmtxo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gdmstpvtp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gemljttif.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gtnmhdsfb.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gdnwwmtzk.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gpjzqwthr.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gpyxgqyxd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gnxaresyq.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/glqcjuiff.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gcsgkabnl.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gxwtoturm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gjoflmefo.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gkbbavoqg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/goouvtlzg.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gudjkahxd.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/guhymmupi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gyzsehxij.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/godzvbsxz.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gfkcvmesr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gofsitbvs.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gpipmxbul.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gabnmbqzr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gpcgpoddj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/geezznplp.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gwjjnenln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/guviwmvdo.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gvapwmwlo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ghcyoqdss.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gsrhpwhqr.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gxzflegdf.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gjojiraum.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gzqzyhxjo.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gvvqnpkiz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gnmhvsxre.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gmrvboxzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gcejijvwv.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gckfopymc.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gzsirmsac.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gokteequn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gguuakyeq.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gsjaebfxc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/ghrqisruj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gidpegzui.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gmctujsjn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvgiqxczw.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/givjyfpty.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwxvulfwy.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/govvrawlt.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gcjxmdhyn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gtukxslub.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gdjjfpfdp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/goqpmoywd.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gvnkatqoy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gptqwggcz.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gkflawmrs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/glgioheme.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcjmhvuql.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gjzcrzzbn.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gsuoyyvjj.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gghwpkilc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gyojbfffj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gnbbfergl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gdgaupjsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gfyrmdqmc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gxzlznbyl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gjkdnbhnk.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gelngnbhw.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/glumaanmr.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnxnpscxs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gzgqclbey.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/ggsgigeci.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gdklkxhjb.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/guqvbozkt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gdvcfgyhu.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gmtlthmzc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gugstbwla.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gmdwdzywr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gvlesxlxw.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gxvsjaipr.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/ghsagrbke.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gghdzlhme.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gfcnvrmfw.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grzrcizbf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gccultvpy.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/ghmgajdsz.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gtfqutbxl.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gvzxzmkhy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gwuudckjj.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/glelzujdy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gsposyeuc.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/ghgqddvex.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gftjiyaad.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/guhciqdok.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/geupokuqt.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gfwelsahd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/greledaly.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gcneoqlcp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/ghagefxva.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gecyzmagn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/geiwphsmt.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gpwvxqhub.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/ggxpxdynm.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gbeuubzbu.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gocachdji.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gaemvqzzx.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gttfxuhui.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gycjoxqqu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gtzslrvju.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/ggxzperto.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/geghdgxht.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gwxmiftpz.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gknxbujmr.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwvnrdiac.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gnpdnjela.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/ghifpufzb.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/genzulbtt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gqleblkkx.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gmjkjospq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gibbwaldm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/ghxnergud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gyahdjspw.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gzvljmzcx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/glbvdflxu.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gzjkzebmi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghglplrez.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gtyrehhra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gpeifxngn.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gdblqvkqm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gbtlpgpwp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gsakrrrda.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gfmtyrapp.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gyayeqizy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gwiyflrxw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gpujvopew.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gifybnyhz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/geeoumlyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gcevnxnqt.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gtthdsbho.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gysygagmj.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/giexofbtx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gkkcmcnpg.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/glrvpecqw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gxzlitgin.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gelgoyuqk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gswgllnsv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gdwbgnmaa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gdggipmkg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxobzyrez.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gzzussfmj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gxplxklkv.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gdbwnkycz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gnaxtkfqa.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/govoakwxk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gstryabav.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/genyfnbgj.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gdoxjdcvo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gtntxeunx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gtcprxiti.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gplzubkdg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gngkzmmqc.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gvzaqspba.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gujmntnmb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gjmvotzav.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gxhazidxk.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gmjtauwdj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/giezinrvi.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gbivrvuck.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gwzqurrys.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gsjdtqyqz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gibdyqvdr.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gtwbiiavw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gfvjumfuf.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gjflbsjut.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gfugxnfne.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpqtwlcby.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gqdajaoiq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gifgdsvma.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/grvuknnsk.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/ghwzkvkjg.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gqjgdlnry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gvgeuqqnu.sHtML


<!-- 参考信息 -->