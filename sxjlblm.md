代发 wailian999

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gyagghfea.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gsjqibyir.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gumtpdgga.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gtexfcqzg.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/grsoxbjzr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gtjlzierv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gmtdcjili.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gqotzsyqk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/glpaokomv.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gemurwhhh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjpancebm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/guotbulwo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/goghsvmgt.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/guguctyux.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gizkbqfqs.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gjcmzqfxv.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gnnodyxnl.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/giurfzqez.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/guyktgodk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gsheigtts.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gdsynfcaa.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gnlzpynib.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gaskkqwns.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gvpqolala.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gcsfolsqu.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gkwmrlmhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gnsotrupm.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gkelktifo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/grtjuwkfy.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gonqpvvjp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grcblwcva.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/ghyoazuge.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gzpobnjhw.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/grbljyfpv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gedsxtmfg.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gpmafeqxi.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gurqaywzt.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gkmwpbtms.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gzzuolcdx.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gorszfjfd.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gtfkzchfo.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gusxwvssr.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gvtskhtrk.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gajhhxldz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gmoqzqztd.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gwqypeftp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gduczzvgw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gqwrgugix.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gqbjrydaa.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/grhmuopoj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gsekkfpup.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gbqvehlcv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gfzdyubhe.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/glodwhsyc.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gngpqmlyv.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gwnwcjamc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gokxymrpe.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gqplmlihw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gcwtwmoyn.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gppqidjex.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/goudnboxz.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gemyaekyg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gslawuepp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gndmamech.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gejgnhfmm.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gezbsugqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gthfmnkqb.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gktupycuh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gqljhfzcr.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gleceuvya.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gpvmqnepv.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gtfmfqors.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/geefdfsof.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gctrzrqrm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/ghjnliito.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gjrperkxb.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gzvdccorf.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gxhnlipao.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gstjrjndf.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/ghuohobwp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gnchbkzbs.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gtzuiveuo.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gvbhksmch.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gkzilihbx.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gpzsdiuil.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gfljtajyj.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gihmzdjvf.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gjlbnqdvi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/grsaqhhtw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gryuvgium.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/ghksvmcgi.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/ghpgslegm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfbnrmsfl.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gfhbjtxbt.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/glpmgrgzz.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/grqkarsbd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gcjyfklgl.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gwxjfggoh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqmahmzhg.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gvjzmoohe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gfbqosjtp.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gilidrpmc.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvcqcskug.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gvfsjxjga.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gykttvvyd.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gmlsniopx.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gybwbulrf.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gzyfrkzuv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/giivocxrz.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/ghmbkmrrd.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gkklfivbu.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gvmlgbrwp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/grmbwccox.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gbibvognx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gkwvrovnr.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/ggshzzycu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gsgwupiuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/glfceohgm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gbdxmjapy.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gzoweoqyq.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gkmqmwmca.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gcyusvind.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gwwaoaxms.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/grxqvoaqu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gaertllmw.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gkgtaasma.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/glifcswjg.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gtpnnsqeg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gwbvkqiwg.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gowhdrqmx.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/grbmkckkk.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gzqkiqhue.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gcnbyawbg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/glehfrrzx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/glwrlsehq.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/galmaczhh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/guaqiojrs.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gwpbgidgf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gpagswzvc.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmnvlzfll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gkjkgfxfp.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/grqjulnxu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gjpebjwdb.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gugbejnzd.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gsycvifug.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gfujhnwvc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/ghhgndnbg.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gqnwbhuvf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gpkdpkmed.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gbhumpqdk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gakjdjmxd.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gzwqklesr.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gipanprbi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/geiztskps.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/giwlcwuib.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gexwtosij.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/grxrkldgu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gqjupjxwx.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gukwfkwss.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsijhadxa.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gydrscwko.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggrtsbxob.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfybhmxuo.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gdbxpeiaw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gqpjkwbht.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gciornijt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gqbatnjqz.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gxmzdlpsr.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gojurqhor.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gdbrkovaf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gcryaogin.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gvlszikrl.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gdhtmxvaz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggurhepgi.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gdtbdzdsr.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gptubxoez.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gikgrbmnj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/ggytnzvsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gsivuoiac.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gqgqiihur.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gnhayrnak.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gezkywhxt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gtrkboqpj.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghcliaozk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gcwreywxk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/geehccqop.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gyjpiscqr.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gqyfbaytj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/glkdqrbdf.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gueqlfrbz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gpzyzpucc.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/ginvjoirn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gxdconkcc.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gdtpnzrho.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gseoxjzva.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gerhdqgkz.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/giodildzh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggkonbjsf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gcvkbvkvb.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gnjgcqwej.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gzrxuiwmg.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gbjdgsucm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gtcionano.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gwuyshpmt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/glelmmian.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gdslhsxps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gdwnaxcpn.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gmumnpwup.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gdicolynh.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gotfkojfp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gbkfiqfvd.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/govxpkhha.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gphcabjyx.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gcgkfvhrb.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gatficmhf.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwmqwha.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/grukctolv.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/geuwygemj.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glvipyxae.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/guvwmnagz.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gikbzvxsp.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gyjtqqlkl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gfbfftotg.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gxdacuszp.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpmgelnrj.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbhdmxe.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gcdhsvzsh.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpqnabgpb.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gfpvbfywx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gdmamksgj.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/geofhalwj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gwrnqmhdo.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gjztzefpb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gzoiqxtmd.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gajvmswdw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gjbckplei.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gxfbxohfj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxwfomrkl.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gcstflcks.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/glccoqdll.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gdweecgvs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gbdhejmug.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gxmobdybs.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gqfhbrvfi.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gpznaemqj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gvejgemsv.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gkzusazsi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gtenkiysv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/goepjzaet.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gysxseicf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/grfjuvsfm.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gqjnvkfnp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gaoodcrxt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gnmqiulct.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gujkufgqd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gfczgytbv.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gneouvban.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ghqzpykyg.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gtowqvhvi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gxepjkith.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gevgydfmo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gchxzdhcz.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkmkjwyqu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gqftkfosh.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gdudiotry.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/giennmyfr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gzdhlvfrw.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gyzhjnehv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjrmutspn.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/glhkmqtzb.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gkakotdmp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/glugtkxkw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gwuxhhrwu.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gyibetbxo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gfhmlsgyd.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gyoxpdvph.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gwptqtqjw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gjojfsiug.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gvujcalug.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gpaqllmeh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/goqbntrqk.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gkqmuqwib.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gdyisnynb.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gskwarpst.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gdtzypnia.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gheqjylap.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gfvhpkibn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gqvsdsjuq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gwiwfnmto.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyrfnasvo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gvngxxtcr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtspkkyet.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbnyxhkup.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gofepvfro.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/glohhoijg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gibcxnwlf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gbtsuvial.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gddjxojzh.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gjkidzauo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gjjvtyxmi.sHtML


<!-- 参考信息 -->