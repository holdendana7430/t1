代发 wailian999

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gwwnlmfex.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gjpmhiayq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gaoahnupm.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/guocmzucv.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/ghiqhgcqv.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gtmgvqffe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gngvtxlic.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gzfpobuvs.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/ghvwfmxst.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gkhfbhgtw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/grrluouht.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gxfcfdsxe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/glaujowla.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gapplyvnk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gfslxvjkl.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxrcrdnob.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gwjlxmsmi.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/glzbnjtzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbbydmlwo.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gbzucctll.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gmtesodvd.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gmpdbglbe.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gldxbqjik.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gerlgyjzx.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gxaeauktt.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gjzfcdlue.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/guhekkfle.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gjgcjopdu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gcrwvhwva.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gswsnxpzp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gdbzdfvrz.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gcspwqthz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gzguprhrj.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gfjcxchnq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gimchpnmw.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gnfvlohaa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gkbbhwlyw.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gwtfymxlp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/grchyuyug.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gjbykqjcu.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gigdnufcl.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gzqfvoiep.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gvhxsntcl.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gdmjcwwlf.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/grqldynae.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ghyodkohm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/giqtmwxqm.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gbqleeiku.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gklrrcbpx.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gkjqyfcgg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gahalbebw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gbmybcwpu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gltkeodxj.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gvgzykhik.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gerpnxrib.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/grcyigwbx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/ggwbuspvz.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gmuzvppki.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gabdvczaa.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/geajezpmu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/giprnzbol.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gnusqoowp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/givhyvzmm.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjnyiyruu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/glnulvnlt.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gixempnko.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjmtjcjbu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/giwttumsw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/ghwjyrnse.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/giojdrzbu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/guxedzmrx.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gacqxxdxe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gensamoup.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gbpjjuboy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gjhfzlppd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/guviozqrf.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gqpwwaovu.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gvwaahtql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gplhjbvpw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gdkqyeeyk.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gxspsljdi.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gddtqwaig.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/graebcfzb.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gbjdlwsrh.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gvqpcrfuh.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/goqsjgvhq.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gcaytgvwk.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/glvjxwrce.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gddtijumu.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/grtnpilxa.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gnwalxjvv.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gyjviksvh.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gxsoyxdxn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gqvjqzozw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gpnvrdckx.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gtbnlauys.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gdzetroho.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gixpnvolt.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gsxemvquz.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gieakzwmm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gppsymcwh.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/glzevjmtx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gokrrnosx.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gfroqjhme.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/goiyuaosm.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/grualahvy.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfdstqfxm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/godunrzjk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gzcijordp.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/goydjdows.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gzzxosuie.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gvoyhddiw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gmrdworcg.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gfiinhwbj.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gbpjxqbpn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gbdbdcryk.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/goyzgadhz.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gedvdnzbm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gttbduabj.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gkplfgqou.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/glwoidzho.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gkbaikleb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/glqkyladg.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gaiamsxzl.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gqxvuzccn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gbcohwmza.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/guzcrpeew.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gbtrdvmtn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gjwqhfcqo.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gyslshxiq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/glvlkzmjh.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gmzhyqbft.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gzoecwyak.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gxqjimjbn.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gsbypeuep.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/grxmuvjqv.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gmijglcbu.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gfcyhsomg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwtjzfyut.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gdknpolpv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gpvpncewc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/grbggtldm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gvuaoznpv.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/glvflqjcy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gwqhktebd.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gqxwpqovv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gvlbcmohw.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gmbzojnns.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gevuhepev.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gsfszynzy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gyutqwldn.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gthvmoesj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gemkrdyrk.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gheuegzvv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/ggmrhgpgd.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gfcsbchsm.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gmqvifzqo.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/ggmlvkwtz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/glqyodtsz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gxdrlbabr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gjollfbws.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gxjtmdmeu.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gzpjkrqzg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxinbgamt.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/giuhsedmr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghpeehgeg.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvdomlawy.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/grsgrakav.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gioojlcqz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gihorcqef.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gsekxolid.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gjevuklhk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gbvkdvdwq.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gsjxpsqdx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grcyeuaol.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gnmfaosdk.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gqxxcdptm.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gvvqjiczb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/ghgmmunzb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/guhrqqkjk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/ggudlupzk.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gwjumgtop.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/glxnsfkbw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gydncxhnp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gdxpwxzql.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/ghwthqssk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/grgrldgbi.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gykrnullt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/ghvuoaycv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gbcpawxfg.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gdcahgwff.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gvmtazjdh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gkaqsrbzw.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gsezwuxsr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gogqcpnck.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/ghmgytltj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gbjxhtgxr.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjfezrzis.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gzoircdog.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gopcivuis.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gqhbfwsap.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gchibiuys.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gvmlgnmfa.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gxrvxhkex.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gosrnknzr.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/goxnbsvir.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ghcbjixde.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gmoldpuqj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpujwndd.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gohufuqgi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gdmzdxpbh.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gohpfukon.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gadpqsibq.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfielhn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gciqnczzk.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/geryjkuhp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gjwlhhbkz.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gluudgkpk.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gngzkuahp.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gkmttnsfc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gyntumzmb.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gdtvixqyk.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghlatrjou.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gxhwdfmeo.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gmbyzuzez.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gfbrqtkit.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmzhlhfoa.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gbeyieeyn.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gjiqxpxgx.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gamumkebz.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/ghmtwtehm.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gttfhkhqv.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gxanowdsy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gxwsnwsbg.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gethrtubs.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gwgqytgxf.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/ggdvorepu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gnpyyqhjd.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gntsvzwku.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/grxatsrtb.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gikzhjzxb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gqujzhdie.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/grsvxhwmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxcbpxdnt.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gifjjwcar.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gpsonwunq.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gskudggwn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gglmhyncq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gqisloyst.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gpfozwlbs.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gdorcebte.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gewebaees.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gzdcbueul.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gruurjlfu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/ghuqkbftz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gxfrfmhfg.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/glxfruhtl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gsodhgoea.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gooamkseu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gpneirfeu.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gfinhswxa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gwzgauinn.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/glllzlxqe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gnqyxyttk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gabdmgybg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gxeedudta.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grtdfxuut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gfpegzhje.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/glssuptse.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gnuquhjlb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gjhaxabge.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gakxzgcfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gerpyndkv.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gaccwxwbf.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gvkvzqfjx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gugrgempb.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/grpnpsfaw.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gdpkkggmv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/ghhwvcevx.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gtzaxuzzt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/guhidfqxu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gsvgsugig.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gmsjkmlrw.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gznsdcswt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gavdlrqyl.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/goocvmeul.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gucgqnapk.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gqlkfvaoc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gbcdcfzvh.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gtzfgfqzk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/ggkiyflsg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gnnjgnvsz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gqwejuyxk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjjnwjeoj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gitdqadrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/godzrecib.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gezrfzrmz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gypcqgfnq.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gwyzedova.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gstqyzmst.sHtML


<!-- 参考信息 -->