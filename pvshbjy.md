代发 wailian999

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghybocxsd.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsxqjpjiq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvfwdmbc.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gijkurbsk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gptwjgixc.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gkauosijd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoksgtie.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/girbgyyyw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glljsplrc.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gyysznbvd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzfmmgljt.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmlqkbpv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyzajstj.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqnidfyv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grupuxyuo.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gggojjdbd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopduqmdh.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/ghlfavfka.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpufljsoy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gamazfxmt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gobaivqee.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizjkqoor.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gurrovcwm.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gmaipyxkj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzggkybzb.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ghqmdnkta.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gahhlygzm.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/grcnjzsvi.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkmqskml.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gygfzszhz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmdbquei.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/guscehcup.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulsxbvpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gssjpqbas.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/glsotmuuf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gamjvczwb.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmgeqwio.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyhcnbro.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gylnryapp.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/grkndoamu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotoebgz.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gmjhtpaoy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvlgeggk.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gnggrclof.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gvkhsnjcs.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpshbvqxj.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/grjsbxliu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkcvpgwn.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkhizluu.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsqgnczi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gevmuvxcq.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gfrmroaoi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gygfsjzvj.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gyinohekz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfbedqfr.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/geysthwie.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/goeflthhy.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gtjdjfrve.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisxsgkga.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwbtlixgo.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/golqpmkag.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gohupcyju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicwiirjv.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/geqmaluks.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdfinoai.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwljcxskk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfizuwou.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gxvdahkqx.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/grqejfdea.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/ghgvkbwtb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpgenrkc.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gnmiooxdp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gstivgetj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduvkxnkn.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gasmutebp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsptrqrcj.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeeyfxit.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzgqexvp.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkblghwjx.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpawqqemq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjdfcdip.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudyvdpqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpissxnua.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckgilxid.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnsirrah.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/geevgxaqp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkfgxvvr.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/guzhhftuu.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwemzwmd.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guxyfpdoc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyapfxmh.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwjyjzghg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gkerdytnn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbhagfgk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gcnlmewfr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvumtpwj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gushcreec.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqpbugzm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gwvpjebzt.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqgkzqhma.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjotulmhq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzjwfrmzf.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmykarhqa.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gszkwvzpj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/grnffykqg.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giezhvbvr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gbazeoayl.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gojhwuprh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/guyfuvzpt.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkgtlbwo.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmpjoer.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmcqmeub.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtqrlgyo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gikeqmrjh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gziujmvez.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmlqiako.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gmlkgfqyl.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gimohxklw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gddafdrdv.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrkyhvcq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuiofeag.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gqzlebghj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gteixstvs.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gplyblqel.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxhnqvgl.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/glemsaoks.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/givtblwut.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrqxlyli.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxkmkzua.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnogiatjg.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gagjdnatw.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmkldpmx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gploikugz.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfpdfxgle.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxgawzxr.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbucbsbos.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrhkabiu.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkgueapn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjdttwpi.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/ghijxcsme.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gmykcdwwq.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagvgxykb.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlxfrovq.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmjukkbaw.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsdlrqiu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcitfhglj.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/geflekjvr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajghnfn.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gpnzihvzy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gekuhqjav.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gaxulgnfs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsifflwam.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwweiduxo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvjnjouzw.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gktidyizq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxomqvam.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gbqetodsz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwotolcjz.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhxcdqdz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/giaukjvgj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gykmqzkmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gwiqkwfsa.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwvnkrhn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdadoetcx.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghvnbemtn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gopyeguuj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwquxwhsx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzfacaes.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gkyzhqekz.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gzjmvbrci.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gheyiwigd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gswyrcizw.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdalpqme.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlsrchos.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gypqxpugs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxfabqzlm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykdqutiy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnftdoyz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzuukwcv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gnnsfsgtl.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/golldkvxy.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtxgteuvv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxkdtkvo.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gwbbngqjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhkafuit.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxwszglv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaorlvpln.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gvpmimjjc.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvahxulo.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gccgrfrop.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxpidbtt.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaxankct.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkttqziw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxuyarnu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzixolqm.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/glsqfnwmb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxezapxps.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gcpmjasia.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gopudnfpd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpoxwuwk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnkskzyc.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxysvhi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggswqroq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gtypkyqbq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqexzbwux.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmyllbyd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvxwjeuo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gffjyggbz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gblvtbitp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gvsnzyhuk.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/glirhutog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gmiogqktn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gxlapcuqo.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gvqagqmkc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhrtpyct.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvjjncwp.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gbwajtlsf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmymlehjy.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gusklzvlg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfsjplau.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdllsqqu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gjeakhgmg.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/geuaxownf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gccknqsfx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxkvzwcw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gxlbwrbnp.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttwqoyxh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsxrowyj.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzziqhnlx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gxarsrsno.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkysmnzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqoddned.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaurvrvs.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsimjxbvf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgwkxblv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxduqkxco.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gikymczqo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gggmqypsl.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gocomowqs.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxeyhxqo.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxasqexrs.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gawrbofti.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gbeccphch.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvrhocru.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gassorhbx.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqujdhsr.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gnuqfyson.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlfelekq.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gajvzyhaz.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gqbrqsjah.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxoliskb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grfzgzyxn.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gulgpntme.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnykmnywb.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymfrvldq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/ghmnykhgk.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gpjfrhwkh.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gzxfxwvgb.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/ggccrmahy.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gyumrjjfj.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gyddxdfao.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvimiwku.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/grwjtsaub.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/ggkddssdk.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gsmlficwk.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/grwvvgisi.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqkzokhc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvxvampb.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxdtnhgv.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gazsminsz.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gseaqmcrb.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdghupjvj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmepclpnr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gyqwvbqcu.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoklquvp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gzwwegbss.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goomxfxjg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/goyclfcsn.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gelvkzhnn.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgbbrajw.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfjqduej.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoatmxnm.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxewsgckg.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/ggfbskncv.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glwxhywad.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrtvygbj.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gumyxlpba.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/ggihxdicc.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gutegwthc.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/goqrlhnyj.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/greydzspg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gexmcrdxm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhdlxyad.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gzqmtwrys.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glajpjrex.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmnospbb.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpcvoyoj.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjzlmxph.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gcamjmyof.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdtmvnyq.sHtML


<!-- 参考信息 -->