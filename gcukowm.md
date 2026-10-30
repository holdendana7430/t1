代发 wailian999

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gzmvpqonj.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwchptre.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbdkfgu.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gutbqyrls.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggqjwsuhw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkggvgbws.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guznemwoa.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwzfjecb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwsmlpsp.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzmwgpse.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwdbhsfiy.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlysrdfq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/glptlrshn.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/grsztlqes.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gubwaounj.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gyavcscwl.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gzqcnvahm.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/giwqpqmdc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrstawzy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqtatquk.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/glueeyqsm.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvtvyuzoc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfzuxrfn.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmddiamwp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghozvpier.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwprmmqc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkfxhehyu.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaujdxwx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnssnnqbd.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gywuuulwd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqdmoeelq.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzldbhoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfgmlbxua.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gahmdpwsf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glovrbbeh.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrdyrnuf.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqnqurlqa.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnregfxvi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbfkskwk.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnydlxfch.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfrpqgpc.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gsoazzsdw.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gokdaojxg.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gencqwuoc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfvcawfkq.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnofcohlr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwyyhfrl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gjcbvhxfq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gaqogbsrv.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grucbvjhj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilujbjd.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzwegapa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gsveazvps.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/grsaupgsu.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gvmbmqcwu.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoedjzgt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gpdcieret.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzlsvohw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrbsefib.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiqmiitu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqkmfdom.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gnuzgbcnw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwevxffzk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpafdxif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/ghstgbhfd.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gruynkdan.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gvipbkvbq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givlwrmhh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrsvtsqb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoqeznjj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/geusdnjds.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxpbdvjz.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/grqovbnjn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gcnthzpnm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbrcoaln.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glypanfmk.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/galkhppwy.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxpwcann.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gscvgaote.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiichcrt.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbihmhahn.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gguppbssz.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtpvzhujs.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/getgiyokr.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzrpisyeq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqtddrva.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpsgsenw.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/glggytewi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoergmdp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkbvgihg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaozpmwf.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grpfkkrse.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyveexfa.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlztboak.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdbsbiqxi.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwrcyfgbz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwsoabps.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaifmboa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcxgfyyam.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmaacqbz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gylvaqlvx.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlaxyapr.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gifflorye.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiujspjf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkqndwxe.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giupvfvdu.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfovitkol.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeiojpfo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/godnhhvxa.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpucxjpuf.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gawyhpwrm.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxlosiqm.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gtkuxaiaq.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfnsfzqjr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gokhnqtzb.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gadzyjwet.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gqpvltaqe.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gxrqfgyrj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/guniiaimq.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/giszjkrfa.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxejcinmu.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmxbnssjx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqzfcdcs.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpsdckofk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmxmcoyq.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxcifzkn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxttukix.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gqvjpqkpc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhpxouiw.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gasvkinit.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzaygupn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gjynjywzb.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/grwchngde.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gtejepytj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geiqzlyhv.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gebgnwfrp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ggzmuyyxh.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gsnrmzqwt.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gipqdfilo.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzxpymnqs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjysifvqf.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gslwujdgk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvarfulw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtdkjvxy.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/glwmfucuf.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gwblkbtyc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goctfhnqd.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsnmpbdl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhdpgeb.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gplzjbrhi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhhzdxef.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gththhkod.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchtcqoab.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/ghkummcwy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtntkjogk.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gyklgsilg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gheqvkpsz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gempjzcia.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfzdxncmp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjgltganc.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwcputdd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gliwgdrqn.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmhenazq.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpanaosw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmkghtvx.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gesqwyjpo.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gpttbbiwd.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhzsjqbm.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gnimhtvjq.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ghkpettgb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gaufaqeyy.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gflmbhwxh.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmimmxmih.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgswovc.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gplfzduge.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmogydmp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhzogbbd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqexmtfhi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gikzoxnyh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gszbvcodh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqtyfgtz.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdpllbwg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gxfqjihqd.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcxxbyjls.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudgnofbg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwtaxcgt.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrmtbbpm.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyyqzgku.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gatkrdxwh.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gylqdgomd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gputrwror.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gyivfdyej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/glayidlci.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekccgpar.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbzmpwdv.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gieoknzbf.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gfmepqkvx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbvtbitqm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmshmjzmx.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnnplozgn.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gmvrxhgiu.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gydyhqeah.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goarusarx.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gfncqtdwq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkklzljm.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxcnvvtl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/grppywwnt.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gfdlqorch.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqylghvw.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcthmqjth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytgtkfab.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlgtbtzd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxeqkgsl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrwhchzl.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/glphfnjnc.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gknujvbom.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gkkueovhh.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvkoqijvj.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixuxtncy.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrbzyspu.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvkbagkm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdwnamen.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsoklsfn.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gwaxgzpez.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gugptgqcn.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsxlodbq.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/graqpgger.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlmnpxet.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gsqrocibj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gehwryhca.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxpkyalpe.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdjirckh.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gmtqwesoq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhscdsdl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmrbswrq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gznxyeett.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gznhjjzxz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/geugirner.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/glegijbah.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvllmlyr.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/ghonzamwn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbuohrdf.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxucjyhpu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqktccuza.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxlusfrk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeciohnk.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/guppcasti.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqfvpbta.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwbqehbm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpouvyznv.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcmguoayz.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gfbambpsh.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeweagcz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbwmvogj.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gpwkdmjft.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ginsvanhx.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gnaocizii.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrxvjify.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxuoqduz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpcawget.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glwfvyyva.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhfpgfzo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggjsbgswb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/graqxrivb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclodhioe.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrggrojj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gezuuumnq.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gssejdhnv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqpvipld.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtxppddn.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/guxelrhpq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gcymnnmej.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqsbjhun.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gokplidzj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhsteikv.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/giblqluik.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gucldnnpw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/guzgftdcg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glkahquvv.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gluhqtpki.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guqoqeilg.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebmicad.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfobtycg.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gerhazjrp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsjtpvjo.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gdogpzgfo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejupxwzp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gokywbrqf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gjeocdpxl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gejotkgzt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/grllpfmut.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/geuvepapy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyujdshpb.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gmxtpbvmz.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/glmfgttoe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemdofdpu.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gdnwehqwu.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjfhdqyw.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeavavjy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwwtvwgb.sHtML


<!-- 参考信息 -->