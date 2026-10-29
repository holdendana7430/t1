代发 wailian999

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gpcqvmcfs.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gzpaekfvr.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gtpkwzakd.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gvyqpxawz.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gzwitrvrl.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/glkfkjehc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gpdmjlpic.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/ggxjvzyjq.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gflhpifog.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gkrqjuzmw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gxoqnxdya.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gwwjbghzg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gvyxqykfe.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gvmehhevg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gglwcccnl.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gtpyfgnjr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gavcfeuvr.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gibzjnjdu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/guckxbuqm.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gpreyaxxp.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gdizuqiss.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gaogwgdfl.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gqtjhpvsr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gcyaytnsn.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gpetnuteg.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gjmizpric.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gjvgcsias.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gcemskybq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gopxnxllj.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gkogtzoev.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gaanezyxj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcguitfxo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpvpskwfv.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gedgwnoxn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gphzavdkb.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gktohgxsw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gpzluqnmk.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gpnxlslbh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gyecsnwpo.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gtxixgmke.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gokxiyycb.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gwkyqjile.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/giuwxcjxd.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gfavrwrgx.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gosggfswk.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gjrhxudmj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/glxazcjym.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/greytvzjs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gdnlaxsyb.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ggiydlfzt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gpxlmmolf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/goyrlaird.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gsrdpjxso.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gwelzghrc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gazktktvb.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gomawhfvv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gnndjdzzo.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gmjbluzig.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/ghjqycsjk.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gbosciggl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/ggchgmidu.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gcggpiugq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gxumtkqlf.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbmxbweqw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gykgysaby.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gkazstoiw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gfzequsel.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gonjihvyz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gsuzdlzyj.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gumnwdwxn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gfmjjiyko.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gpuvzuqmk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gumnobxyv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/ggsxewnzc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gsyvvyghj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gwojxtuwi.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gpspizhqt.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gpshjfdxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gggpezmeq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gqdunzemq.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gpyxmuskz.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gqyqwyxpc.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gcscvajiz.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gofxpscql.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gmxctzffz.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gmnejbpqq.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gxafcpzgp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gemwfsokt.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gamkznlqs.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/giygffuxm.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gtrycjoxk.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gxjngcker.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gkyoqfqlv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gxatdgaum.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gdcxnoplm.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gsrhgslsp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/goglssnvi.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gomekpnqm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gplbrfbmb.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gxkldqgsh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/girsqhysd.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/ghffmoaum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gqnahlqpq.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gllhgioot.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gxcapwakj.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gdrbuuzlz.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gctrzyazd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/ghdxwuxix.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gzmyqdmdh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gsxwxcutn.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gxorstywm.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gtgqydvch.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/ggigxqyjb.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/glslaeghp.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gdfpwdpzg.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/geevsymgs.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/goprpolmp.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gvjbeqcsn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gsbwyxdsp.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ghjpqumba.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gczdqhnhv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gvjxlqwjw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gjgujcrjb.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/ghvfsweoo.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gwhicslra.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gengtivtf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gvznxmads.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gqfcxsmhh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gtmkjgeay.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gzgqeivdl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gkgwylmpz.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gaugklxzv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/godwqjqku.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/goknxfpww.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gtoltgvpq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/ggytygcdu.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkeakkr.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gyhoqaxjd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gglwweruv.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gmhcgsyfz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gtejbbysc.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gwvssegnu.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gkwvpqcew.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gycqbtkjd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gkholimkq.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gzheofppy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gqcnxzxfi.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gynoemjgj.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gkasxawzo.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmulzbm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/geaezgcxb.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gduaxvlba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gcuzgitkm.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gusvhildj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gsxtihtcz.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gysisruwy.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gcynhoivv.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/grwzmximr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gpifdfntg.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gcpzfjzsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gwdolwhom.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gcjiojrjs.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gshjstogq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gumqmcykd.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/ghxewfhfj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqzzmvbte.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdbagyokj.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gxorspjql.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ggtxgdlui.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gbjlcteuo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gauilrtob.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/ggtjezywu.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gglqqaudq.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gqxhsfsij.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gmmxwolbg.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/guokddfps.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gwcczllxc.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gmjxhykrs.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/ghnjlxdqj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gzuhgzjzn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gmcaqngrw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gwhsacgwm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gxziqdlci.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/guiigtpup.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gwkjcrecr.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gvyozpmeh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gtcpuxsuy.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnnfavsze.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gdbjzzvwn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gmhfwdusg.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqcqnxbar.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gzscjmynp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gokpnnujl.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gpulyfiuq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gehgmpylu.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/golvtcizb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/ghshnqttw.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gylysdbgn.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gpdrizpit.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gefqrcklr.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gillmzxou.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gwhfquvft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gakyjydwi.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gdrdrvfcm.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gvzhrbfxb.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gpjavzjdf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gdavcqedv.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gnbdzaptf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gzknlhema.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gbffqwcvf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gkssmnkmh.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gybyliowt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gxggzzfzz.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gnisamtlk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gbfxktpry.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gsapypykk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gszkyhhxc.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gfeavhfjs.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gwehooqsn.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gagutkbky.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gfanjdztt.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/ggcvpueym.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbxtoltdm.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gvffvjirs.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gscwzxwyu.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/geqcbrudv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gamadhljf.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gdirbduqc.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gshslkpdo.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gteqsjsji.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gcexenejp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gknwqoaul.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gvlcpfgha.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gfjqfpfqr.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gakzbqwto.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gefviugwp.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gwxktlmby.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gjaycffyt.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/giymifvng.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gyvrnosnf.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gwzhpofzr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcxarsovf.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gkyqdtaop.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/glgkkvlcc.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gwpvqmyzy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gmjwjepay.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gjpmbrcxe.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gssaxjnxy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gtruixsmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gmxgxcyxf.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gtdxwatlg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/guirhbdsq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gcvknduxk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/groapowty.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gnntwnszb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gwbygcute.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gzhhqbgbg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gmfnlnjpt.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gkmkohysx.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/glwrzwifh.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gcmvscadq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/goslfbpey.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/glmxecvgm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gymdrawvc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gvcnnkriu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gwulqgjtb.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gctfxuvij.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gkwclscjj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gnxukooys.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/geihkqctw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gkmdzpvfx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/ghchqxkgy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjjbihnke.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gvnlogkwu.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gymvyflln.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gadetnhjm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpchvfzq.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gpfwifszp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gldweobfo.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/govatqell.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gqfwxzctg.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/ggnvwgxfv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gkrrktvwg.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gzblsbkzz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/glymalzkv.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gotwohhlb.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gneqgrdao.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gfttvkdci.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gtjkrdmtc.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gljotcwjs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gslxpdunf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gptcrjitd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gjadwmuza.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gctmrbihu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gdwhguaxb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gchrbazfi.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gijschlwd.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gesqvnrsi.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/grspkwzid.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gjwgpcspz.sHtML


<!-- 参考信息 -->