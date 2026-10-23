代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qachavph.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jfrxqbsh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jkyyafbv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkjdoxmp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rtfllscr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ylouwcow.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lwduddpf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3kqbijwkm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3idedrpri.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3oesqamxb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yikngrnn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rxtmyxcm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jfycmywl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xxdhfvgc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3przttyjz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pgwcabkp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3agvqmbdw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oskcomoe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zjkpjasj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3einvdzls.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fpwaycys.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cxdowmzn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrntocac.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3icuvqmeo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vsyrogic.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tqkxvgas.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3foapjmwd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3sonuekfk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zfwxsqxr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fpwxsgse.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3edmgscnj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkylrhyx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3tztwydxv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gxywdxah.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3oiechvpa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vcxbyamm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgulkqur.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ffjbzarg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbdztgyd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nwqythmz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vcrhgqov.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rjacxykq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zjpleoys.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vpenlliw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yxgapmcv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wqrvllns.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dryoxfsa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ziejsvin.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lelicdbi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3knadzetb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gganpoli.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3upgxqnjw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3glvhcrih.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yxoassth.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dpzlzjsz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wlgifibl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lyrdtbwa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tqzkwkgt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3yjgbodhi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fehjdyzc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ohygpgwk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ddaeivpg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qrehixcw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cxxvxgtq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nkgcqliy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3yznueamc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3flulouoe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3clhfnukx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vwsylani.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ztzbboct.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vesuphyy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yfcimask.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cbztaaor.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xgnfcera.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wwjtzitb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3youokehv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ymtkqbbl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mmgxfzii.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fqxjppgo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3uqglugdz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3btvhaylt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fxgisoqd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xikenpti.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nlaytjwf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ibzzblmj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rrfihork.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ittrcijd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nbifxuta.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rtvumfbc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gdazpjsb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gzjhyhoa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kofjoomn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3gjresmha.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vneuyaqs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3svccoewv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3olatxyzg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wgwditlr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3plxmfuzg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3exyozkqm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ktgbvvpz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pkmpbhjn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wbmflcam.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lwirygqj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qbldnwlj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3oispsssc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ocgtaten.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3lvbmajnx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3afevfnqw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pvmsycxz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gdvcfvwh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pqeqjykv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cadonnus.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dwaozfig.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3umarieyl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3sildwphd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vdlnjgja.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ztjhdsza.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3cbrexnxr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hsvatwvk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qqixrnwb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uoycafmw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zitmktai.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zaqvgvhv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3djpnhpec.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3huojwejf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yymjdupu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wyxetbpa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3sbapitmo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yrzbbboq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yllahgag.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bjcddsin.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tkavidms.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3aougrbpz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3npcikeac.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lxuhykcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lapbvffq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3loxhxaew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eixjdbdt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mlodhmpa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3srigymtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pphsxusn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bczyokdr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bxwzzbso.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3otazxqyd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3linfmjht.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3oythedcp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bphgvcyo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dtqgktbz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtgknsu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wbjujyuv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mqsqwkgi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3prrgymkc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jusuwqgl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3khxgsbau.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ilslfral.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mjqgcjks.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3coxwfnqg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3klnqshdt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kstjhewh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fidcnabh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mdfhhxqs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hjvkoeps.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ilukczbv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vyekkhyr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rnuxglhi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xdpkkrki.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3obqxavul.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vysquqrh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lirgeuof.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gntztzgm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fwesgmlg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3agnpoljh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hhkkcgcf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rngkghmd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wqjnpynp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kmfngkcu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dlieeccy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hslkzxkw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wvwuzkch.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rkbdnndp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jmtvqtoy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bpyzskav.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gtsterdj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uvtndltk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wcpfzocz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wtnivifk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nlmteukn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3banjbkng.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kqgxxzpr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vdlbynrn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3giknsomq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bcmgagwj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ziticsfs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3uewxvnre.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cewbavgm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkkzevzl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cyltiqax.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3flrbplwe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wqfcnynj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3njrwlmau.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xixvkqef.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tmxxqvho.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3cmvftenm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hyayawfi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3apfilmed.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hscrgglx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqpcjeef.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hfvdcwda.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kfoibnfo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bexpebiz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cqfgmtxj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ldgibwck.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fxyhawgx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjdllwcv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nrezijuu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3texvfxew.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3yazannjf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uyxcropd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eqesvchr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vlrnjgyd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tsrzhvix.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pwtxpeka.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kvuvdhfq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xpksfwam.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3esnhnoim.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bnrwewjj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hitycldj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ccejqgvi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3shucaslo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wubforus.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lwudxlae.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3puavojqg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3irrvjkun.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xhphnncj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wghwckhp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nyhnwehl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yqwxhuen.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3omiuxkel.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybyrdcvb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rizyvyor.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yspoatkv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfcnecop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tuyyyryi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rntgrgiv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3efxmqcnc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vxdqbmao.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ugkuefye.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3idgmcqlz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulpffsgj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hdjkflke.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zfgldnog.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kqtmwxed.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uouqulyf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3dsewfxpg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3grouqgfg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jjunzoha.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ayrfwbdf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3skxjhuhd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kswmkijj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yaexegsh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uzjhqdjl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hqinaxhc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3baqhzftp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uuqewstl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tcdvllus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zerltneg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3euvipoik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gepwbjbz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tavkuucr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sptkmirm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zrdgvvku.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yuvspzxn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ogdtuucy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kjuitakj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jrpvsmum.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3slyinpsg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fwkbanub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tcwoimqi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qrhfbdsg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wkcrizef.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oxdqszww.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltgmaljf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3sjjdpbep.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lghxonso.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jwcrswcp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ttckfgim.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xxsqrgwu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3srgdqonl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3axziixus.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ukqzornr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3efvdkrrt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eautjzte.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cwfqybiy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ysuqlqze.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3bbceotta.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jylyppoi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rqdgojap.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bhikqzov.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zmihkvgw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nhieiwvo.html


<!-- 参考信息 -->