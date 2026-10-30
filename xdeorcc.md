代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfzpvspb.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrtnmqke.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcsdoavmb.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gapxwgqzb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqwmealwj.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjhuranlk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhlgxyeq.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlptqsbr.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkjfneqi.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkanmaabr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwsuujdi.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeoylkyq.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsaoibdl.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmgafwvtq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcvnxtrwo.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtrfmpij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwkofaii.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/geqoslvbr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnywqrito.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/glwiqkaeg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmvoyljre.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqputyxpx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkokexzik.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcydczsgm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqvazmrvz.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzturiot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywcbjxnc.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/guryffnkc.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsyflqlgk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlhtlbht.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjwtohyj.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gveaeholb.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghntdsrsc.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrackvis.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtylhkqr.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqnemozry.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzinxctm.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gxcnhgwoq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwcvucdsv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gddhgqoni.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlthiqvi.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlcsmxin.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/ghfvelgzv.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtdvqhuf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/goteyxwib.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpcsplvm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gpglpbzva.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhjeppey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfejibtyi.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/golgdukoz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gzswdppnh.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghanrfhmo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlbpwejj.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/glquryhca.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmexahdnq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gxluequov.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvwwmfnn.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gocqqyhxz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/glqmwslbr.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gregsoerw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gjkonytnq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gllcnzocs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gdjlzhnrw.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxujysexu.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gexrcbism.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqtivskr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/goljzgrrl.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gkuiachcs.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gugtlshax.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxdlbpsw.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfhlynh.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gymbcvori.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gavkulyge.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxfvhtze.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvtvflbh.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmpqtmail.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqmbyovt.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/geyounwua.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamtbnzrf.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilicfvnk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzxbjoro.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gmqgkwcrv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneyjthyr.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssvzaxfv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gilicasgc.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrwduqbz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvffwscg.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpludqppt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfbpvdpf.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfegroyf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gotgbjtvt.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/ggmhimbps.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfbsvlgq.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gtovubmwv.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmhpetjlp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbfrjqqh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guheueavy.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjabegrev.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpuflkui.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuuhvbcr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqctscxy.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqanhvcuy.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/glckmkmhm.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/geepamvwd.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gyvksqcyr.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkscsvcsq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gzwtsuerk.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gjsnzukgm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gfhroitpl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdewfbifi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/grmmfliwf.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrhzffkq.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gmeanimtb.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/guruhikdm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaqeeyxn.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gpwqkmdlm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gnqtumjps.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gudkdllnr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvprpqrpt.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/grisetuqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwqpmyaq.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gseklsqcj.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gkubuertt.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfowuyiys.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gyetzkttq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdvxiajj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjahxuxo.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumofraqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gtkvitceh.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gldrekqhd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqelzphiy.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghikowmcb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gectjjxuw.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaznwrph.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqyquczwt.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhwbsab.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxthfmle.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gpcgyteyg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwigdpaks.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzfzqdul.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gojstlrkk.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgwbxlwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gsxccettl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljfhdahd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotqxnhpk.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuzgmasw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwmykstbo.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoyrbggc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbozhlthf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ghktfyibo.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gfkvnprtg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghgjjwecd.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzpmgiyq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gllejhspn.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpqefstb.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gfyvbxwfk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsovfmjms.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxrexjdbq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gmomhnmrl.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gboalcmax.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groejkejg.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaxtvvll.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcsexckd.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwhrkuam.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzprozmk.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gejvvlhnm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrqlqhdb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhiqqcnt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gegkkdbob.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlxaaspq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjacthtrt.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gldbaupuq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gdtvaiveq.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/ggajfdexp.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdvexaru.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guaiadnmy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gxacvborb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwijmsaq.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqurnpuhn.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbvogdpr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyebdokm.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/grspnowvq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzcalrn.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/guotjvucr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmyjlncn.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhdzrni.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gpynpbfts.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmrgnvaz.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glrvgliyd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayxydhvr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goknchbgw.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwbbnpni.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gngtqqmyl.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfylvknww.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gvotbqfcw.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdliquyr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcdwxwht.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzfiufon.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gtciwngai.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjxgsurd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gqsdyilbc.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrlbdzhx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginnpxttg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyxhnkmh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/grukqwvnj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyntvdimp.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/glupndgzq.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gnqsuzuzk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzzkpvvkm.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gpayqnhzi.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gztvnjbqt.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyircozcd.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/glikloxmz.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxaxmvpa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gihuxbmng.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gentsbfxg.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/griyblmsf.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndzctfbf.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gdovpymxt.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/glrlbpfec.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyxmhbup.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrqcxip.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gedsusoky.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqaruvv.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gnsvwraui.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gkubfqrqw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhjujmye.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gncrglzgv.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gcuqlukay.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/giglaixtm.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gtrlhorss.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzmggyrio.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gcguxvaqh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ggyfxypcj.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gszbghkpj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gmdkhaccp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gijmbmaxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gyicfesbk.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrbgpivg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gutfqcysb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiehodml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixupxdta.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gizdpjndz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpbsfvqj.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtdyopey.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/geknpvjut.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gxvuzaant.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggrpbejxu.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gitzdclol.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gouvfxmzh.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gefjshukh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyuraegwg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvgtkhzeq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtksqbxpo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzivexxmo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzahhekz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/glirddjll.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcwgrbeld.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gvteyufzz.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvoonrvpq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gjcuuuuja.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvsdfyye.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gxjoqines.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdwwdrn.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqugdgoea.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwmknfgm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjcliszu.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gknmtsiqr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnhvkqolc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsijsesdr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gtaafwvbj.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gletmsqlt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfajawqn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvdoqkzg.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gxehdqcah.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdrfbyen.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtobrpee.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/guqlwoxoo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/ghmsiaolt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gwasmaxlo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycnqvmis.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnsjczfm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/ggsgxlgai.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guvcttqhn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gifvxzpdp.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiwkdqkv.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaxkblao.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcghtkit.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gndxbyimy.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzszjpduh.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/ghwyelbre.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gtffekfoz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdqxoqoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gshbwfzlq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gjynusckl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gejmdzcxt.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdeuerccq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gkgyjjzcu.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgrgvwnt.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/girneowgf.sHtML


<!-- 参考信息 -->