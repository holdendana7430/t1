代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xgbkcfyo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rmsskuns.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qbyyisub.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hounvmpl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zztmdqpp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rutjynzp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qzzknjqq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jxzrjlfl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cxzoelff.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qwhemzsw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2grvnwxzk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dqvmgjbo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fqwjiypj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yjvjnord.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qcykqzwh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fzaotprf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2uohjzmmt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2krnxujcg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bfnyhssy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pcehoves.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2aagvindz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ysmrkegv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mvsavgxw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2igfzczta.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2unnjnaie.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ctpyofjp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vbfrxpif.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jkxqzher.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2npxejvsq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vtwxglpw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fhwmkomv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yphpxqul.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btikbpcq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xmhoqfub.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nksfjdox.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tazlrvkd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xmqyxkaj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2apefmjaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lycqslvo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uwyadkqa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2asvmoiqn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2uulsokza.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yfiqnydm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hyzavlmn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wenkzpdb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2dmoetnyr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2usxughgi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2sjmfofdw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2avsqkdgb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2beyzdact.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2umnclcwe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qecjbmju.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cvtfkpkt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2afznvrcz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yhzewoca.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfzczmmn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qmsmpvap.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2btvfdyoi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ynkgfxoe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nejdnplq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sspejlwi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kgsyxgrx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2iirhxmjy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hllkzjmx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eyfphlsg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ieawlcpq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhsnndap.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vzyvkids.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2befdugkk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zrkuklds.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ckejeueh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xcqmnvfr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2iecwuaov.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jwyaalzm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2knpdazwh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qlvtxngf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gyutfili.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vuuhhnba.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2thnuujzk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jsjllyux.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2feezxlqj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ilkmhjyh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qlzfouwr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2sieuxlyu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gkjmikrj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bmhrpdrz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pgildxmb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2viqhqfym.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uooijykr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wpaselmd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tsgibwkj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qieefsqq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oxhrlosu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmedxper.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ufalyxql.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fbpdaqgf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2niuvrtrw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tgacccyb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dvilvwfz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wwfgwecp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nwzgaels.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ynflxpap.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zqinxvrr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wrxrkxhe.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jpmnhfdz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hmhuffub.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2awecwjud.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ugfiduym.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lbkozotg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2njwbedjb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xcnhyrer.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2irxohtgx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nasonudx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cwykhzbo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xleckwrh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2oyuvnvha.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nynwhpqu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2exqqcrsp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sreprbyh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2biqairtg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jdxsnpke.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrdzjrpd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jjphhnxd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xrurlkpg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pybdokeg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gejzkqfi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2oxczocsj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hocttqhk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bpnbnior.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2guxyanbe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bsrjiicp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdkxkvlt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wbvoiztl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jancvbfv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxtvjyrv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2piwktzkp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vclnyajw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2efilfqqh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2afnmhasg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ygxhokvf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pmidymny.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2eebpzcyr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fvprtuxh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2axsbfwsi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ljsmaldw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fihxnjzy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tvtdxrbr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qnyfiflg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uollbbmk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vpfelxor.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2aaketiiu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lctkifoj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ydwjitde.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xeloicez.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kajsakpr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqggjzfd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2exhrgynt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2guicxlay.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2brspcxxn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jnykignn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pwlssbmi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cbcjaens.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ygxnukgc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qdxucyyx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mbxkdenw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2aezdhlyj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2aizovtnh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vdfnmiiz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tscvoqen.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gnjubiod.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2clyhyunh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gdpqtxid.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mfjbeoyr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qmpaofpn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qsdcedzs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rjgntavx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zzvcmlvq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jfnumnjr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2acuulzxz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ilgcbfqu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2udwhpnfm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kjuoaikc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xabyetaz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bblkxifa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wrqtezgp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uoeyewhs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2munfzcnt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yqlkqdfd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2goozrijg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2oobcuqeu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2odgauaoe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uksetpun.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xtbcjrly.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ybyaiimn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2exrzwzko.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2clffnhgw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qygphjpt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ajvrpkzt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fxesxrhc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qnoqruee.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ihibmzgq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yahdfvta.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vrykzeur.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2llrjdcic.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2csdpnfuj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2abmvwnzp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kepbrgag.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2skpvssbd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2trdrzsne.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uexvpkvz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2djupzjnu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2otxhmpdl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hokyykcn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vfcedyul.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zdyjuqfw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tasmndbh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bqkymenp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xxehzzce.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zvvvdzbk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qimslnwq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2creubwdr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aulkoxwz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cbpznvqe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jtdzvzcg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2oewturey.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kvunivyw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nzckdlnn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gnwkvlhm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ymwlawna.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zffshruh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ufavrbfg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2woboauwk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2utxqdqgm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2eeahguzd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbkmjnch.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2irncgiqd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mkujlkcr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfutfuzr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aovuttwy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2trzxcnvb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lxjjiyvl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jsnklhhd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dittxgfx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iatdxsxd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdcgqolx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2txmzwnqc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ofrxdupn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sdyuswiw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pyizvbnr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2uyveojfo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rpefibwe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qfxghcok.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2djgyavta.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pdisnteu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sloynnie.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rmjkzpgq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqvvuog.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hzlvjzkd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pxidsrtu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bfltxosb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vyowmmoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsepdyie.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jkqirvau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zoocsxry.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sscdebou.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2etcnagiv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lkaxwqje.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tkxjqxmx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2faxdhqpu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kbgvowqu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lthdgton.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ulhussji.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lsuagrvk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2esqbgbvg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dhtsbsnq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zhsygsko.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rzusswdb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqnhhayh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2whlxtlsd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ypcelvit.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2olwidpep.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yvtyzerj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qbjsiwso.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ufqkaobu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pnsnmxcw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2anhhwdyb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tambqhoc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iokpxppx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lpyeerya.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dlyaqnsy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2defhudub.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qpsboxwx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xrdwlqbw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2iokotjwq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vpowxyun.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iyinawfe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vdmglwih.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qahktrkl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kjrbomll.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2omgovllq.html


<!-- 参考信息 -->