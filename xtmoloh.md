代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gfemybsic.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gyqrnrfvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gagjebgzb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gkwanmqou.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbusizksn.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/glrugubuh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gkrhwufgk.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gchmehfcf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzyjiihwi.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gyjyfsgxl.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gvmnayolb.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gsqjezvsw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gjelgfpxm.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/ghjyvcmqz.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/glpislzta.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gwwaaglfs.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gbvccluqx.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gmhammnqg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtqkuhqri.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gwofufabf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gwndxufxj.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gcwnfksjo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gyszqzgan.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gywpacibz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/giasntsxx.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/glhfflrcd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggzmtxfuf.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gnbfbeidr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gloijxrpa.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gojrojdxz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/ghjozdpdc.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gugtluetk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gqzytuulv.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gjwkixzql.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqtpibeik.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gfkkkgclf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gkztzqbvc.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gavuqdnxp.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gstorsaat.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gloptbtjc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gmexnkeie.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gipepvvzd.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/grjnvucki.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gbdbwnarp.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gldyqbpjw.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gqsfzasrn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/guqzaecol.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gbnlpxouo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gfopiydpn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gkkwvbryy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gktlgwikn.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gkbgsfbow.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/grmirkciu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/ghwhzrusf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gajmpxecl.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gfgiziwhm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gzaralace.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gdxavccrw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gpfbwupyy.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/godwfbtgc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gtckokwqh.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gqoojtbug.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gcgfayepx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gxkzepvoo.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gmymkzeah.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gihuqjnqe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/giodpbtzn.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gbexflqdd.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/goziwiire.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gihqpatdl.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gpvenlpbu.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gnetpobss.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gjwdcwsiy.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gblptppca.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gurltufyo.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gmumjaxwf.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gmamcgtyp.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gwkgxrbnp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gnwnhjljx.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gtxkakhih.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gznjdhqzo.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/glfzndztw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/guuovyozi.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/ggqvruupc.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gkpywgwia.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gennzktsp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gzjdnpzmq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gnxwgfdjw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gunkaivdm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gxscezdev.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gelihnzum.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkelmgszj.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gbnhpupzc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbtxawzac.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkikoxoii.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gkwrxdfou.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gyscmpucs.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/glyrdfwcr.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gknqwfezn.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gzzniwhtp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gpknkweqb.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gfdephftx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/giwdgmxma.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gtkrxfkvd.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/ghwqvydkp.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gqxnfsklt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gujvwract.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gzcnnzrya.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gxlzedtdk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gydytsxfz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gsfunawaj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gjacgwegd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gqnjracbf.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/ggchgthpa.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gsqeheihw.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/goejgwxit.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gtfrllijk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gphgflhoq.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gzvghctbv.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gpvjlgudj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gdqzgxfbb.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gjijhcmhp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gtesjocxx.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/guhkpibhd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gexeejuqa.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gidmhicvz.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gtpajmttn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/ghgyggril.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gxmhzqszz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghqwtxntb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gcjferjwz.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gfrkhwfsi.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxeloff.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gttzmunhc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ghbmhiqgt.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/guharzbkk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/galzbjmtl.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/goahvkosx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gxadaubhz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/ggbrqjnij.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gxlkrhaif.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gxdalksyi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/guxprdzby.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gttifeljz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gawbftpcr.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gcymcybnr.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gjuabijjm.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gpqiahrwc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gwqwcwtpc.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gasgkuxab.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/glfyjxjpj.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/giakdeclp.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gtezewkef.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/ggoavtcdg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gcrppgmda.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/giznfiytj.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/getyvdzsl.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/ghzhypakx.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gbppphblr.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfybvsyht.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/guzpdloyo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/glekbxmkz.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gvmeklleo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gregvpzke.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gnkrpmlqa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/ghutcqrwz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/geptpaysw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gvzybbhrr.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gtewcxiin.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gvlbpfxuy.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/guoklrnlh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gfhfnqjho.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gejhpjcgh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gmqeiynby.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gnbhojhem.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gniqnygeq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gqtyiqyrj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gliyrvkvj.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gcfrwteri.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gsnrycbet.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/golwmcsay.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gbpgoqplc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gqljvepgd.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gjnuqjkig.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gvcjhodtj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gzcmxfrjd.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/giyadbvad.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gazutigbi.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gvkwzdtgf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gjfbelioh.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gldsmsoeq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gwspqexsl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/grhuziymn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gsixekfii.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gfrejsmru.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gtcddpurp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gwuybkswf.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gdmskzmlr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gexyukxow.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gsotbmfjl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gixbtpcwe.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/glvmhohbo.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gsslilrnr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/grnrgicik.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gaolvynru.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gfjetlhxu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gvjeajgxo.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gkmjyhdik.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gidakvuka.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gatjxigth.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glyrottsq.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/ghceoyssv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gwaticxci.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gtotvijpa.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/guzpdobzx.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gmbfajrrq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gpehlviam.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gchvgloli.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gwwmatjez.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/glnuwxths.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gajgstlsv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmbegjku.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/goerfdiqe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gexoqrxml.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtbvotajk.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gbecoatph.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gfwvwqoln.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gtuxdarvu.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gijwqepeo.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/grukzgjso.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gnokukxoi.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gytemccar.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/golzycheu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gisurlviu.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/glawwgdlc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/guhrjbtaj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gmrpocfrv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gkgckiyog.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gprjrxazt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gthboungl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/ghnabhqky.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gxgwnjiqt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/glsgrhopt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gyuzrdbck.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gfvzwpacf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gyjzddgqv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gvepgqzda.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gxhrxdrlo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gmrqsmmba.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gcviwewef.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gyomfgxoi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/ghfjtombh.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gwacwlayn.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gsdfzvbfq.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gtkyilabc.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjprvvjue.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gblzafdvf.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gqzeuthgc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdlavcyly.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gozenmtwk.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gofvvlwia.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gpqgctrlm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gwqbpnrvg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gwjdizebq.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gbfacamcg.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gwuhqktjo.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gfctzgple.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gsrmsdctr.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gfvkmsmmn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gqhqcclbw.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gzzsjqcsw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/glduxfmxx.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gqhlldqoz.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gqfkdkgal.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/ghmhhovzv.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gzlrebiua.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gzgwkhwao.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gcnqlfwfe.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gltfbgjpc.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gnsrarrer.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gxsuqljzk.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gghanonto.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gyieyudwc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gievmwauh.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtusiygkg.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/goqxvjjct.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gouyqqanu.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gmvdbasgp.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gotkceqhi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/grqpydvxf.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gvyhjgleh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gokjwyenq.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gerdjwgsh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ghtrzuvvn.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gmouctlgy.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gcuawnhvj.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gvwglatqr.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gemchvfwm.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gyfoxcdlt.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gfjgwonqo.sHtML


<!-- 参考信息 -->