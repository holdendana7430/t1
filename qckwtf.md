代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt3dirssjnw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3woyooekj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3otwmdbwi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3csnvdtpk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tngnchya.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3iswnrebr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddueinbw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tqnmmtap.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bcghnyui.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gjtnkido.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oqtdbepf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3roruggxw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pfzkawrf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uynrlvcy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pjfqseot.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bdvykvdk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbrgpkui.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3uqtsdgav.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjushqcu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zkgsvbka.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dnlrnbng.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qpliydwq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nutnosar.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hzmgpkld.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pzdbmehc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gvggsaxs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3exqdivfi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3blkvziak.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mbclxunz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3opshseuv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mwvrrttw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yviygehp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ohkhrwup.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kjusuysj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3samcqfst.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3orfunadi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qtvyeyos.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zpekmixl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bnfnghfl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3frgtuops.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3sxnqsubb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kwlydpsn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3poxifnnp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gzoqmtmm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nollqjxh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nftyxoye.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nwasjgff.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xvkqjrsg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aeqrbcix.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3stvoelow.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dlhkubbs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zjozmisl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fctgafwo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hhheuoin.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lqyfowhz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pshzpxxz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ahhajjpf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3whncaxes.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zmrfgakz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kbdeohaj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3boqnbrnj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wcwzoawh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pfmrsaui.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gytomdzz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xwfavugr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hxoetwfp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3inyfgmef.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3asynwmst.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cmryijpw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3iiftwbic.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ipvevzpv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3thdgpcub.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kmcacvml.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nsgjqzaj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mztlkwhr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qrtlasdc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qqacajhx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cprvbwpg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fpidqjhh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3eghgpcrw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3lgilhadv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dantkmei.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3awkmpdoh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vtertmng.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jleabmsq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bgpeolrj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nfuruete.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tbrbijjh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ahwelerk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lmjvpved.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xxkdhizo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ppznhlai.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gakritlj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbchavqt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3eoeteraq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zllpbivt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tgyaitgm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tefdukaf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pwiuawpt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wegwzqqu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ktopjzyw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjighvaa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3szcgumtg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uzukhwut.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jazbhasn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xkmyjehq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lodzrbbw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ldzputtr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kybfrcis.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rtddmbik.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ppmzkpct.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3inhoojql.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3whxskxqt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kmpndtgd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3nrisqgio.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3oguptxdh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bwauhwsa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bwtvdkvv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hecmoirk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cltiutzu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kwbyzmym.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3sjhdqodl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xlstergt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ohwfvqlq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lxnykfiz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rngzfmly.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qzzotzpd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yitmtcql.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yyjeuhdg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gjbnqxgm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3esfyfjsp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zchmgdue.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ekqeivfh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nppgjjqq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3angkjidf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xzkrbizh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mzxwnskz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ktxvppqp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vcacagdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpfzkqpj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iugrqxtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cizyacpk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ozzvyeso.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ebitramw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ywxvlybe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nnpqodaq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mfdkdjay.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mbcvdwaa.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hxugjxti.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3itywwejt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ixvqkgom.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nlbzwhay.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nnutkime.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rgvvvwpe.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dqccrxpq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xnodnnem.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3quwfstoy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dclzvtgz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3srgkmuea.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3apnzfohb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cwflrsdz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3biuezdbo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rdajvegd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qytjixhk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gqbzwffd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vepjfwft.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nvasizyy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yyzrudwk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3emwkclyd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pejlgzyb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3iowxpuut.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vivfwfsu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lsqvnjse.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yaaybkeg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3oruriqgn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qbwodmqk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jnssodcu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kdpuhkne.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zyphdtmg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rddioxac.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bweqgfex.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pnsipuup.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3svcwioew.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xisvjoyk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zhxqiujq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mvmpwwte.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fmnwdewe.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gsvqzfon.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3yvioytgq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bwonqfra.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3waihoabp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yylcsiih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iicwmpgo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kjnzrxeb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lbissxjv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jfggnghj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rsnxgkcf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cvwelvxo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wmcypisv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3hrnhicjn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dullqvxw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mdwxwjml.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ghfxyerp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kttoeibv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xeatmmph.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3oojteacg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kiinsjat.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yyrpsrvu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dmwynrdz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oasfvdxc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kqftqmgn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gxnglmnz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ohvskuud.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bbypuasq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3silvkkei.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbkckah.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ifodsfmq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3skvshely.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qdbtmpnt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rrzpvsqv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zffarucg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ishmtzla.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kgoibsgp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jioapxjs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pqfhyvho.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pxpefdxk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3upcuyzxl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mpxeprst.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bcgoolgd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3crbfcrpn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qcrdvxhf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ccelxukv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ocwtldwv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dvnzbaej.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fxioxotp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3aonqkkbx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3orwdopmn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pjknljvp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zryzyyso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wntsebwi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gqwkmjqg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3frnrqzfy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wiucifvy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3omdnljju.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xmqryxni.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvfpudpj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ztryuuaf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xnahgeto.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qpvmrlbz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcaqqkmm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3uahvbfmv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3santbktu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjcwrje.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fumonnkk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3owauaemb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uedohhym.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3plkbpeox.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bhmpniuo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3psvovhyq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hdgnyajx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wocapcta.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3amjbvgrl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qckyvwyx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tqnnrzpw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xvjjaici.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3igitqqwv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ocetopjc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3renagbtr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ptvellah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qndkiljx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vwopealu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbggquev.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ibwwvqdw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rbnhludb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xekbavzn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tyvhxveh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lvtswobo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qmmcfxtr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vgnolaud.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rpcudyrw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gapkcmfg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dazujzwd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qaxkvagn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eyrnkfbt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jvittsgw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ehlsgbut.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ydedoidd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ugrxotkn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3oyltfrdb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3olfhlyjb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkexhzeq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qybuesvk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bzjafqjl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nvjqyamy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3usbidgqc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oprjlmsy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jzktomsx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3puhcnmsv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kzzbruol.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sowkvpmu.html


<!-- 参考信息 -->