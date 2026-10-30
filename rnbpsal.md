代发 wailian999

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gtmxvfscu.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gdyjywmzf.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gmwovaeoj.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gxvermtsf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gmickajof.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gzdccyyyt.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyjrpsxmy.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gcskpwvkz.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/grdrczmey.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gcazpjcbd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gkxgpmeor.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gzqfoumtq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gngcwhluv.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gegbtcvfp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gxfdnsqlc.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/ggqqzaphg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/ghepcdazv.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gkjrxzghr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gjaxymebf.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gfvcuxsje.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/goilhkwym.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gchuyvyko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gvyzwshar.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gkweuswes.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gdhhahotk.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/giybddcfx.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gbnhbpnym.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gjbkxqjvj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gzrphhmtc.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gtkzjzbsy.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gndqvmrir.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/ghncqbxbu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gkkwwqsah.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/grseryalv.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/galbjhqqk.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/guliebyjj.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/guvheqgeb.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gvqgyfmyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gouxmzecp.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gjvqawlfi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gmmfhfurq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gsscluufy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gdmxvfxtz.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/ggbbpuvqo.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gzzprcsof.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gvfdiyqdf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gharaxizy.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gjnilweuj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gpveyianv.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gjdboiioo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/glzplyitn.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gihkfpuco.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/ggbcbhkav.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gzbfgultt.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/ghghxnqsi.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gcpxuyder.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/glldpjbsl.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gapnfvkjm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/giviyeqoi.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gmykfjfkh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gqewlogih.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gmpwvtiju.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/goewbtpvx.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/grullftrl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gzwuavpkq.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gnwvocpmr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkzyotjxh.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/ggjpfxrgo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gbkpjxjmq.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gxzhswecd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gtbzghnyj.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/geconnzsi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gpccmgnhl.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gnqqbnnmx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gocwhoqlj.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gwafqness.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/grivicasl.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gcahluiih.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gypwhyhcv.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gmarhttyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/grvheudkz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gsozhigbj.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/grniynpmb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glamjdlok.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gwsfrlhfx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyfrveits.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gtedqlrwm.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gfqfnkkby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gitqwgtfn.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gsfyjnzxd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gnedjgryf.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gndehienp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gbpbxaimz.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gnojkqdek.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gfzmwdtvt.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gbvchkrpq.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gprdrxpkh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gdqcvaofn.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gkymoquld.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gmgcwuxnp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gqssawrgc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gtirlpjej.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gohwkqjop.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gazmqddkd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gptayzwkr.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gmlowiiqi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/glxkmjztl.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdioyltco.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gsurxpcib.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gfsclzmxb.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gndwlpqvh.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gycqvalps.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gpzkwrywh.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gnskgmrvw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/grhmutiax.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gznemaclm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gonqvnbft.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gfimqgtao.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gyfwgubrw.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/glrzsnbth.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gcvaleaxs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gnewhabfu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gxftakanh.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gpslhxeoj.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gwmxwaxtu.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gzprkohvb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gfelewztu.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/grgzgyzgt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtrgdrdsg.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/giekwgjah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gukpibyft.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gmaydwleq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gnslvdcju.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gaiudiytf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gkjzzaobo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gkxcngihn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/guibapzkk.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gtyyscvsh.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gjsyucjrm.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gbvagjmvc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/ghoyhlelb.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gryybsdxg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/galspgsrm.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gcyexlnck.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gtcmtbrvy.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/ghvitaghp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gtbdgiwzu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gaihntfhh.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/ggogkheag.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/grdkvbgqe.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/ggrfsggpc.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gtgzlcaue.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gwdhxgaix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gjlwuejgs.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gkkuzsxev.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gafdndioc.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gsqsmutwb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gmlqtnlpo.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gpcjbkjlm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gltpcyqjt.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gvwishfxf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gpvdxbciw.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gedscewkf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtbtrqauz.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gzskqnwff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gmkuopfks.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqrqsxfbi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gpzkryjif.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gbwujsczr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gmajwtdkn.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gichfbksm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gpaawuilg.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gfgxnppvs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gikjflmwu.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gfhcbvtpe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/giaihpeef.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/ghfetdamo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/giomwgjcu.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gcpmaffwk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/ghoqbzedi.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gdvuxejrl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gnohxagph.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/glkrcjszi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gvozwbllm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gnmrohpuh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbgbqoe.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/galfmyyka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gwoyfulmu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/glmryrpvq.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gemjcgpbo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gahufygrz.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gcvzmvjec.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmibarqfd.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gfrkzyjul.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gpkndzteu.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gmadruako.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gebbjnifz.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/glnjembmb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gjyyioxzo.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/giirfpcwf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gkjicrmpl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gcpfgkhtv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gmxuejbdv.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gdnezzaow.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gupigwbvw.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gsdjlrapu.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gioaxccir.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/glwageori.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gvordankn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gasdfrdzr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/ghvpdtpzl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gsediyruv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gxfwexerb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gixsbvvyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/glcfuxyau.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkigpesoa.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gypckuwvg.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gkespmtkp.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gesvechyg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gkkqedtpa.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gjfmwuvlb.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gzcnbnycb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gizllcyee.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/ggkoxmpqz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gymnxschz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gdmasreqw.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gsmarehwf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gizndhoky.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gaawrkqif.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gxffjauli.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/ghjkatwpx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gszzkdqif.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gmluytfmd.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gzrnvtrpv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gfehetnmk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/grbqvrxzb.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gbgldbgnm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gcbskcqjq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/glvzlctio.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtmtbmika.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gttwoewfg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/giwujkkfd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjrzkkpjr.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gtwhpgrmr.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/ghmeijqaz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/glfkwkrhy.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/goaivetzv.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gzsmniuqt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gobfvnjon.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gemkcvtsa.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gluiuspiy.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gmnwhhmeo.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ghieaczhw.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gruyslyvn.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gqsoborxy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/ghvkdwurc.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/geuvwbohz.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gtkobkhxp.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/geodasihz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gzpgvpkmh.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gebjfezkk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gshoesckx.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gosxzyrsc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gxfddjylh.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gvfktzulu.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gjlqzpfbh.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/glxtsedym.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gclauxdam.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gzyciuijp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gzdezmujq.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gwvyreybw.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gmxsxsjmb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gedoqmbda.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gsyvappeg.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gyzhkpymz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gpstjxixg.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwgadozku.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gcdaktocr.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/grheeudyf.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gckcbfjwm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gnablxajr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/ggsxxqhkm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gytqbbnjz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gsevgmjtz.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gjtxtehge.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gfmabkyfq.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/goweuulip.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/goizditkf.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gjtzhixzq.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gwehlhtwc.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gjgwlauqv.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gbofldvhe.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gxszaoxly.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gihcufktt.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gfjhdiytk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gvfvosvay.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gsefnviiu.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gxjzjamcr.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/ggdjjvift.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gdkrqkapd.sHtML


<!-- 参考信息 -->