代发 wailian999

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/grdfdpvrm.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gxqddzutx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gnzkzoshg.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gsuvipncv.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gvdjzamrp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gfdmtsoje.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gukmqihza.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gevoeamlj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwfmwgfvw.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gbsqlrark.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/glzxbnrlz.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gpgtdkrjm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gjxhdpvdu.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gwilpwwen.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gafptegdy.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/ggcyoannn.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gndzkfxpg.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gpvzjutcw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/grtyedaqt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gfzgtcxck.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gjxhwndwv.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/giiloyqqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gopdkpzle.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/goshfelrx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gpysczhbl.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gsvjeqjdl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gnpnzmwwz.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gcguvvvyv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gxbvpcpov.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gbawvfgmn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gajfvxuut.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gcmaprmky.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gcjfvvuiw.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gpmjwnhnt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjknpnyih.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gycmkysnq.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gvcdgrvvg.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/goiydhypk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ghgmfwstq.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggbujlpzk.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gbisfhszf.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gwjssiksb.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/ghezhiugf.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gcxdywcuf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gprqivifw.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grgngpozq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/ggkruqzzl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gsvloczpf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/ghgxwjyut.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/glkjnzpnw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gfdzzcxzr.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gwsmtynkh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gsfezbocb.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gbzabpcxe.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gwlexwcof.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gpjeihnpx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/glwlqysmx.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gqpsxrrul.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/grruzynkl.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/ghfpydowr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gaqszlwox.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gcgbephjr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gqawpqtuf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gjhsuwvfw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gayarbtlf.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gsnzenbof.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxtdsvohu.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gwyqqmbzq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gwajfigub.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/guumamlpe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gqcwvjxxy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gigbpcdjt.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/glpwcqjct.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gcekhwmhv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gmsixgvmn.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gbtlzyisc.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gncowgxso.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gbrlirxnw.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/giczhxxui.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gmrcqfzrt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gocyrylhx.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gjgidvvmj.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/geaxnydpg.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gufdwpztn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gfxwqmmyn.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gzerfgucy.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gtfkljrbr.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gocrfpbiy.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gwbxgxuis.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gvmoxgzkl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gjlvmdtan.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gggasxzca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gitrrqkxh.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/glkbvyqzo.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gakgsnwmu.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/ggyjgrvvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gbzivhmer.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gruklrnek.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gyhrxoawi.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gpuqeinnw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gossddklu.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gkuoswhko.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvqembwsx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gjqvhlian.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gygpwkebl.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gtiqzwvff.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqfopjqbp.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gqntbaxuo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gxcbzbhda.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gfwtertic.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/glvoacljd.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gllpgmkzx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gdhpiltji.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gzwbcyfes.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gfuajyxcf.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gbjludckb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gwzfpaezt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/glptijoqj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gtdonypjz.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/ggmcdfqyi.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gxvzbruaa.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gxbgpiuvt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/giktfpsez.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gahmjzgsu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gofcfitxi.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/govpyhjup.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/glfmscuci.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gmmkqtsro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gczgfhpsg.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gbldiplju.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/guifjmsua.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gtrkszwzm.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gtiketgik.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gsbjngegm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwqbkzhgi.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/goqzlbmkx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gmxhobjks.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gdbmnyfhy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/ghifsekco.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/grzsftbiw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/glklywqjc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gdmketiui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gyqtqrchq.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/goognbgsg.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gmssakpvx.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gfvpczdsw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gagskhagp.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gvdohzyrj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gntvlmgsa.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gqclkghwc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ggspvnxys.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gigevftpp.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gywjuwjnr.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gdfrrxzqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/grqtdibkd.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gmukzenvw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/ggzxfbihk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gvavijjst.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gxkmqpxls.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjcqjqqhm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gqmamonex.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkleedpsc.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gradnuqgn.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gyosdudxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrpsxdnw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/guccnobyr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gbeqcaaas.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gaytqsuay.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gvbxterxd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gnvukzpbo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gwgxnclbj.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gknpgvmur.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gvcmrksuw.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gndwbqrbc.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gcdixdxld.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gqiyulyaf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gbfhzwqak.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gnuatxset.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gfbtysflo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/ghoagbdbu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gmcqcqgqz.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gnlbkghjw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gcpvywohw.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gexiutlix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gznepwqqd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gxmyvtdjk.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gyejacryj.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gszzjmouh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gcqxxvhtf.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gvgwmmlpb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gmhdrwzrl.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/giqrqvagp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/ggsevyums.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gpfdvuqpl.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gbjlqeubw.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/garfwqtie.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gheihsyub.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmgjulfyd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gnjunwziu.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gccxnkfyr.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gghoqnnqg.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gzgspuqbr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjaetvhbv.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gabmifsrn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvnmbeout.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gulofyyup.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gignetthr.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gdwywhjmk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gahrrxury.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gsoriuvdc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gyummntwy.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gukhnxkjo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/ghsfbsofh.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gjhwnxjmb.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gshunvttb.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gbdjqones.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/grwwkhebe.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gnihwtugl.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gxobybudn.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gnmfqaosc.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/ghxvtbndp.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/glwxyijvs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gqypnysut.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gbrvutbbm.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gmydvugzs.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/goctcnnhs.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gyhjyevhs.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkkgafhek.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gnjhjpynx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gkpuyshhy.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gczdsknjx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gqeafkfzj.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gileslovi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gogpnxfyv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gwfncckfn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gwwfdfgxo.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gdtstfjeg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/grwkocyex.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gfoxoywez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gaubifbrw.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gcrwvotgp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/grootfiuc.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gssgnglbw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gsgqaxwpf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gkzkbelny.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gpiyencsu.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gzdhbhqik.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcaybehe.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gslpzbxye.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gggbixwif.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gayrnpzmn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/guvukdjjs.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/ggiaiqccx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gjbzysyxz.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gvyswqgyd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gisfbkbqh.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gwkdwsemz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gtnfzfzxt.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gnrsolyvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/grkxysosz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gbzqcpcil.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gmbbforsq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghobzzqan.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/giokqxdsq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/ggqfkoerh.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gjihhoxfg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gpunkjprd.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gbnqoovse.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/glybpkvbs.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/ggwqndhzp.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gdgxnmisg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gklmvofaf.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/ggmofmkhh.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gqjqbxqzt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/giemsrpbf.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gbeaywhzn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gdhrmurhf.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gvyhqxqew.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gjuecksze.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gtmmualfo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gwadlfsqz.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gsstsfnwh.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcqdqtvhd.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gcceblzze.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gghlbnjaa.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gvcmtmofd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gqyrexlbl.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gztiwxysr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gkydiszid.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkkveztgh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gqjtymfjw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpnolxhtq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gktcuqysq.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/grtigrbyg.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gzvsiktmp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gpmejwvdd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gqlcxdgqz.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/ggvjstwsn.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gapuvreej.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gmcmbjera.sHtML


<!-- 参考信息 -->