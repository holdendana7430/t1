代发 wailian999

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbqesxzi.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gxordiwgk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxzvlxdr.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gafglmoie.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnvoxbvi.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gutriprru.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzomedbm.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gminamxsl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjncytrw.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiyjgiol.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfrcqssy.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyqaviicb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwxwvtlb.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjvhgjgw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghgtzkxhv.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gsypyipuh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/grqhtnqix.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpamvwysd.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaxnfbgim.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoedtsgj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfhndduxx.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggifdyhno.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcdhtvgn.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gxlxusiqt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjwcgtkk.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gipralohx.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkgnkifl.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gxdrgahti.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gcukczfvd.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gklojbrlv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/grkbexznd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjwtvrx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gzilvnqmg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpqflpnc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gqxczccnu.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/glfzfybkm.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gqhluidbf.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyzuohhhm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gjhrwanhc.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gztcmrzux.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gotwubddd.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gilclbrhj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcqvuvwm.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/grbaatmkn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwsqhjsb.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/geyjpfqfy.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiqyeudb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakppqjwf.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvylahyh.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvnucqtq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqniauyjb.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbdmfuiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gqjqzthdy.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gyotwjakm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrpuzvdz.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/giconstcp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gooidquzs.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gphndnaew.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcdvvkgs.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyyczifh.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnechoyi.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gpzdcpquv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gccdiware.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpyaxytw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxvifuyc.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghbmzetxs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gpowwnfes.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gbgaarsit.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gdigcudcs.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/ghbaaqbjx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/givufwkji.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgueqzgj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmsotkns.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gkmvtdbdc.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gflgxsmtb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjqtypcr.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmfbhiek.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkubchuue.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gubfmwwqn.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gakgaaycp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gthwpfjpq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmwuvjud.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/godgznqyd.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccbcnefe.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gddfgaymy.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gskelduox.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gqmrzjwte.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjeesvmnc.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayjgkwdi.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gntvvtqzf.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/goqfljsae.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnebjjyq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbwxznmq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcokpicc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/galgwopcg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gsoservbl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpagtgrpx.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvxoyggi.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkhxczvk.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjuwtafh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gbhuytmwm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gqddblgmm.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gieuscgbt.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gimegmzfd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxmfbqcy.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkkokjwb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyoxkoym.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvotnwc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gzbktlslr.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgnxqsxw.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gqaljwcio.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gumlcrawy.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkdkxfkp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gkdxguqjp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gljrihjil.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjwekesv.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoinfnbd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuyucmex.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gwixnpnhu.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gutnrsfii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboorautf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavddofmq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnlivwuk.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjzwkqy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gtttqmuji.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gxzatwuua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqmhyrcl.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gomdoyssj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwurwhfp.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gtcrudpyq.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrhsqosa.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/ggndfblai.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gshhkhaaa.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiqeowym.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifntrshx.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdosrzfn.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gasdsgcak.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgidvmse.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmnzakpb.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/grabqpjdv.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbgljpsz.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/grjpztjoh.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtnaxnzh.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzwqoprcm.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhafrhjq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzxggslc.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvmpnauuc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gurbhddtp.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gdjzwkjzr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/goszgikat.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gfnughaeh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsmmcsqz.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gezkxtmbh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrgbaamt.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gnzhjeezo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfzgfpki.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkofjvuk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedlymztv.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/geiyhvyox.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ggcrzrwji.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtkzhwyzj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gfwdldjdw.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gucwnyime.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkrnxmsy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzakkquxc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnpljowj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzapbwbr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gtktnsthw.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gunlzndbj.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/getegnkbx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfukpznjr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsantcstm.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gbpcukhlb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glpwdmhel.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gixplvgbk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/geamcivbb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxplpfreq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvfeyzzj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqflahvhz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glklbkbkz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwuehdtcq.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfjzwqcib.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gmdpaobyx.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghqittlws.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcnudmiz.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gcqleuqdw.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gvdzejkgr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gcqmabgmi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goalnrxtj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudblyqvl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gserwihli.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyhfiyji.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihtvgcsk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gimocbdpw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhuhjzjq.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhsryfqn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuutnzng.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdmorzhg.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkvfsthg.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gzndbbkfx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprfoumln.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/grnykvpxx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gucaspojd.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljdxjrw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxhytkra.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmbxliqpx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfmivevf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giggpnzwk.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqasjlukn.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwhrhssd.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsmwdpnfi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulhiiyec.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmxahsfnk.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gealvtxmz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtntdgtrb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfuddqtz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gfsumiisf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gcglfnldd.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpgruecg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbseqmnm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtlhuunb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqcfpojg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdliaodja.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gygfzwbub.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoqvmjzm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhqymtco.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gycbydmhm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/goxkqfmyh.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gcswniqji.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmayddng.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gpbbcmnjf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxvpafwv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfpvuxvb.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwnbqway.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gygrwczdn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzkljdap.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gobfjwmfs.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gumqvmyhl.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjkjwxrj.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gouzdcozd.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwrswyqlv.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhfjjhq.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdluyqvjc.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqtwdout.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gmvdivvia.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbxmxsxc.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gdafzhlqx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzdlkpwq.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/glxpdufsl.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxwtgqhq.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/glovfofxi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqccotdb.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxphpqqy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfnzhjwm.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/glrgxncbz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/godpusxbw.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gwduilmme.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gopozkvum.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gsxfwrmkg.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwkqecvq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcqhqctp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gszgwblsv.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gduytcoij.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gutcbnwzy.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gwdsehahe.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqsgcbmx.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/glfvwwjrs.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gwqgmujrb.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gutckzktz.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqznhyrx.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gljkbaobi.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gajojbbve.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnusfhmm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptrqvdci.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glppbwmay.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgqpmirn.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gyenfrdcy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzbordzgt.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqjnludqh.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqnqumrd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuvlhvqz.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gyxbmlbyf.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmtgsgdy.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvvabooh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grszynpbd.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gypoqagfe.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gplauzebd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmuogsba.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gojdaanye.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytyagsfu.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvhjrfjl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/goymtfgxg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgomxlib.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqnrrdfg.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/guislisqe.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guyrolhzv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlwqxttu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gogpzvkzf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpcoglpv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzogyafh.sHtML


<!-- 参考信息 -->