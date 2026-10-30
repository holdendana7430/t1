代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ggpcpfdqu.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gdcaztdpo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/golgewrxe.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqdbxaqpj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gfmgedkiz.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gomxuluqd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gtoxwbpgx.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gdbfkbcig.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvtngscbv.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/graevqmkj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gebpykaql.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gngdafpip.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gkibtmtdp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gwwyjqvqk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/giwkslexd.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gomkhtunn.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gugiaptig.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gssjusvmb.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gzmgsaxqj.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gqqabmfek.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gezhkguyy.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gwmuhaieb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/ghhgkhuee.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gsthrwgkj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gbagvjxlh.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gbrumfhun.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gunicnejh.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gxmhtdxrx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gawhgmllp.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gwmrukoqz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gzmxrqafr.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gphnxnfns.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gyclqnfgr.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gwzwggokq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gglkrgejz.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/ggqlyxzdi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gwmnznqai.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/guiwvxbgo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gktplpbfz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gzyprtvxf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gmkbedcmf.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gpdcswvit.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/grilcgyfz.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gamjhuhup.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gnwrzevck.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkywmtagm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gjhmcpxkz.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gpzxsfokt.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/grrqjmurs.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gnqnhbgks.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gtwcksslq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gwmmaiqty.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gjhknmfoh.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gptfzqbci.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gdhxlystn.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gnxcwwovj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ghuedvnge.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/glumhzpgi.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gdserbqdm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gabnmgbno.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/glwqxxano.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/griayjicx.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/getbmzxfd.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/ghsffdrhd.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gjxljjvwu.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gkjqheraz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gkwvcwesj.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/grrlwtdyi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/goziuhybs.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ghzwctobc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gmawxzllh.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/ghbvusklr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/guxxsctrn.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gvjtkipdq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/guptcligx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gibmvqgsy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/glryzxxrc.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gegzwjpnq.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/ggpdjkcow.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gqpxotiay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/ggurjccji.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gspkoxalq.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gdwjmsjxi.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gkgibrxhz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gekzltsxf.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gajqrzgdf.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gajcpxtwe.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gxwmayayh.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gbqhughjr.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gzwdqxygq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gocrrzyjg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gzuitjqwz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gieorzjdg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gvupzwjnt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gcfcmvcqp.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gonenedop.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gfdrsaodq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gphycixgi.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gqvhxfpvh.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gnfcchihg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gsdyclzvf.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gjotlmtpl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gltqupvvw.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gfctvccbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gvulaqbso.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/giilfsvkg.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gofzfyptt.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gmcchflir.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gzwrcolej.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gpquerucv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gjcvvleqx.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/ggvrytruk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gdssmaaep.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gwdzqxick.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gothremgf.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gelmukkua.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gfusavlvj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gatuitfdg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gbbkntxdd.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gvahwvexv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gooyhtyxu.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gbiuxgkie.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gmilvcajg.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gmffeuuwj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/ghcaqonan.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/ggrziqgam.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/glitqruwb.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gzuhglsti.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gelbnqlqc.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gwazjvqyv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gzzacmbed.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gjpyyqdam.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gjjhlrkve.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gvtiyjwmr.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gvgyesppz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqpybazjr.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gzbazerdl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grqcfbxff.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gznopkyty.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gywnhmboz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gfvxzlqiw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gmnlugvkg.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gjjrkcnnm.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/grmzndpww.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gyugccljp.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gdwgbnumc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gnokfcury.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gcvborimr.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/goduuxcwj.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gfzmoubnb.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gstwjlwtv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/geesmhyvm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdtmlyypr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gvacwddnw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gvlhqzjjr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gasefptvg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/giabdkwyr.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gkjqeoffl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjrtwzxep.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gneicfimq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gmzzthzws.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjhanwgu.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gczhugazv.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gidnchhsy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/glectlxwl.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gxomxnwzm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gzjfisvgn.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gwkrncafo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gakcpnxvq.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/ggxqmxyhs.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/ggbgmswpk.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gcmpgkwrj.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gzmylbaqv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyzxawmrh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gxmnrlqqb.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gaxqdsaqs.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gglyhtksm.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gihxppbgh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gjddyobbr.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gaqolpikb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gyrvxnplq.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gmkrtzibu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gtggujlgc.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gdqhtkczc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/goslnxwud.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/giojsrxrd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gjjqmosdg.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ggtseweee.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/govaofopf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gglmjcltj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gejcgqytj.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gngvfnugb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gifwoyihh.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gxjunlgbj.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gldpkcjsa.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gjecqvyfi.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gssmkrbht.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gabtfkyah.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gxbzgugav.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gagxvhxdx.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gkorqruhb.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gfqlurygh.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gdjwawyvz.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/guduzytxd.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gduphvtbn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/ggqwphpom.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/ghhjetbea.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gwapgnrqv.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gwrehbtdk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvxbnmnea.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gtymwrciy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gidtrqftx.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gyjuhwmgk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gumbwkbsv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gqgeyxpbe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gekjglqqm.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gggenfmrz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gufpgzabw.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/grqjlcmlf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gikyaqfau.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gtepppitr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gguwphlqc.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gepmbjzxa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gbitewnir.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/glicrdiji.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/ghqjwcjlr.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gjygossph.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gdajzvamw.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gfzwkyjgb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gdbkfvibd.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gtimnzxwy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/ggiwsmxcz.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gdobmenkx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gaklpmcjp.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gmfykvedk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gwuzupugm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gvoizfdni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gsjzhcmwl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfckzaidf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gqmzqzzay.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gnsczmwhi.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gqjmofdag.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gpgsniphh.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gdyyusevh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwhrhdhmw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/guzhfmefb.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gpllgteuj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gumtullxz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gfbipubkl.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/ggwurfejt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gvrzssbja.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/grxsonyle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gfrfydafl.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gwpvenafi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gsqkqalpt.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gbgkqxwld.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/grpuhwbuz.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gwcnkmlxl.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gsukspldt.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/guhdsrmnd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gafzvwtuy.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gvpzkejja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gvyonbrim.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/geinmgzdv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gqchgkxxp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdhskwwbc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gojriwnwi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gshctbaou.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjlqpdwax.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmljckoiq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gffosxpim.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gchshaqmw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gdmymieoo.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gddzbrhmm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/geyphouhw.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/ggqnbarbi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gazkoykwu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gcwzwbxxl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gmrulckgr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/grfbcbsug.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gkleipyop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/glpmyqzae.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gqfcolgjf.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/ggqlpvinb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gtsueggoa.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gvwmsckos.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gkbmcofwo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gjbmjyabp.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/greqrtoyd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gesvnqepu.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gcbkhwuxt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gugxsaubs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gucllqevr.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/glrcussas.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gwxhdqyam.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gnppnkzql.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/ghnhobrsf.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gmhnjjhae.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmzkbdjph.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/geavsudlg.sHtML


<!-- 参考信息 -->