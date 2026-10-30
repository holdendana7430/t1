代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkjppxazo.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfolivaa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gsevnxpeb.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxmqssrq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyryimdrs.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbcfackc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsavgsrph.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxehlwhe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gpmicribz.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/giqfatwrz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/glxgqclyp.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvtxrgau.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gromuddaj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gkqsainax.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/grzaphfkq.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjhdfysom.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgaiovbn.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gjgwmygeb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/glzrxtfao.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gmjoroniz.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gnmwwyghe.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gyksnpbog.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnuhfyib.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gfomkcfnq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfklzrhbw.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girmsmunr.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfsdrdbj.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guevkbuhb.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gxiprgavx.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gmhkijthn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gusxebghf.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gfbkgokyc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipvzwcao.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyvyfpds.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwytdrert.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhtedfmr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggkrnklvb.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gegbndbqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gogxubilf.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlzduvmz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gqucibglf.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpcyfrvc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvhbdfkdc.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gfzufmkql.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxaqtboui.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaivqhqo.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvbsltzbh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjfjkzqh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzcjldpx.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjtgmcrov.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldxqnofk.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gqrptercg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gxijhdzpn.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmcayydeo.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdapojlu.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/ggnibjcfh.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ggeagattz.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/glyptnqnc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/ggruzvcab.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvhjoxjm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gjthpwofg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ggoznblmm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbbxxvxs.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gifcyllsk.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gmpqusopi.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghmwpiazd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoztmpvt.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gizkepyrx.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/geubzdjaw.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gatjksbpr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmacnepz.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxrzjuxst.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/glmrjpocg.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlsecvmx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgendgsc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjhyjgzo.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gampbiplg.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/grfimxtza.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqljvlhl.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxoltyrr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwwvnuz.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gbrhfdfph.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gfmuryhpk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegdzhoah.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbtbvups.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/glajcdxxx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmpqpdfi.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldayrlm.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gmiylifkz.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gergspxxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkfrufwhw.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvjrbaaj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gzwrirefd.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gojqpsbcm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gvnciilrp.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/grspksaph.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gvcwejlts.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gscciepzb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/govebkbla.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojhoewrj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcfjmktwu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/goekrzbsm.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhhlwtov.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbfoucqf.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gowixieek.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiososee.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghwukwfnt.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gbpmouulf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqjantou.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsednswwh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrscsdna.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcybltfkb.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsadtjxrw.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcitdtch.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gagvrknaz.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyyaoqgb.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gioukbzfv.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gluhecsib.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqebommc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsigpftvy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gybusumvd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gzzzfpxnr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmridljxx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdollflwz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gdelerggz.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrtbsmz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gethjvhpb.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggizaqwqv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqvweubh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/glpouymtl.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbxogvzz.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzziudvfe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gymwluesh.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gxlkkwjxj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gznizqvgi.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gykujsjva.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemqqwke.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gijxwmtbx.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeglvtbx.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/glrgepory.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfjwjrsd.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdepzuwtq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhkmelcd.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbpgeuoe.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/guihpndpb.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gqndjcwfz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvcevdkjd.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gotekdouk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpadjjopg.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gcqlzsxpb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiezjzjl.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gjxckdgyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gidyeoade.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoauxwsw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gncjzdgmr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkgwwbzg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzgouold.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gejamppwk.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gpgaaseul.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/goekfiefk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgxndhpw.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsavwcpr.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gggnzfuvn.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gczprjkqf.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxkscgzr.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/grhdoznrz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/grewwfopl.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/ganfpxqvv.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvdzivud.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiwxtpjd.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gypkdgizz.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfixuecbh.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/girfperhn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghsxbquqg.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxzogjrwd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ganrftjmw.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnjrbuud.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gdnnouqmo.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gfmfuqyrh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnrxpbcw.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gbpuxcqqq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgaqtjgb.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gxgxjclre.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnxpvfyj.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gwkzscezl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqpfvqrxw.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gnrlufxnt.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gguuitgiy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkgoyubi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnbctseh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufjwnzsp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ghofpsuke.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwtjsopbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpspdrdtm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyvnnuiec.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gdzzdxcea.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gqwvzafvi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwgcanjs.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gztjqagvj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcomibcic.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gtqkyqfex.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gqqqgvfih.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/glalkdxss.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/goipcttrs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/grijkxsbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gurghxuow.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghthlrdej.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrkaxoxg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gyclviuke.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxecjwerh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggppvruae.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gimpjpmxz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gohscnidf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwymwefbp.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfsglkwi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvruuqgb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grojcttat.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxinevqqx.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnzigtrp.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gefcisjnx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gbtptxwji.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/glomndpnj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gbekxkbfx.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/ghplyckuf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfczphek.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gxtsmmyqg.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glfwsdway.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gxfdbykxe.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlxetgcf.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gmhfuhcbw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gnvmmmzcs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkmzwuxh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gksuxuuok.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgbywnin.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwevnana.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcknpaiel.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghaupqgdt.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzcewzzw.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrowjeom.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gzhipskmq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/grushavfg.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdlphryw.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gnhgblyue.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gumzcrhig.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfosigxx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gcsmgqdiz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtafsako.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnuqqnyy.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjkcnysov.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/glaodpzzn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/glbqioejs.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gfunhirlt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goictjhfl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccerspwo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqkntvkq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gdfzyqgvr.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gcxpuhipv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrvbksdp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjsfcsxj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grlwhnnjj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gmjfsqroe.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvpafujaw.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grudqgagl.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/glznurzzs.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/glisslafj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyvgqlnp.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqgoxmiej.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqinckjht.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamneyhpp.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyijimmen.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gntpctrdi.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gabrtuiin.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gudwvaehi.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscfrqlfj.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmerbbho.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/goregfzad.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ggczidsev.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlapnhyj.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/grygqztuz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsxlabhuw.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdffimep.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsagbwjc.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gpozojvim.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gextlqruy.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/goelogwbj.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gdzwyzhtv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgfpyvrv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuixhmcm.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gesdkdgvn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmmichvdv.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimzwoak.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwdbcwia.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/genpwmzhx.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gqfbjmihw.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gvufjcfnp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gefulyvyr.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzedlkzol.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gxizpxafr.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gntmbelrt.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gebonuyut.sHtML


<!-- 参考信息 -->