代发 wailian999

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gibixcjtl.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/glqljdhax.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gxmxifixs.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gpeqtabow.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gzcwtxtvw.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gdlkozhew.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gpidzsiia.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gadsmlnpn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gvpopvtty.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gtrwbzzgk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gpdurrsgp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gyrnwjiap.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnlrxeulz.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gadjmpiga.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxzrmrbaa.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gldoeuryu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/ghbmubuho.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gsppwqvwx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gobyzfgxw.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gnprczshd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ghcmdfaks.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gvtlclswd.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gikxerxmo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gcpkqbmus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gmhojpzhi.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gnpgosktm.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gzfgfprdi.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gwozkopkl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gstnjexbq.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gyxktdqqa.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gbqvtfllg.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gwqthswdm.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gtulxmyxs.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gtxzrifqe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gxdglmrof.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gkibjsayv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/glrlmjdxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ghotcqrdr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gdyxyhsuo.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gejbcnhad.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gkawamvzo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/ghjjlnwah.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gyggbachc.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gmiaaoyeq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gjdhevvjs.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gxrxojoem.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gtcbkavex.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/ggatugnhs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gpfcmyevc.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gfdxunvcv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gjduqubmj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gjfougweo.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gzntfnjxy.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gnyuqgpwa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gaesjteex.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gufxelseo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gcalvufgg.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/ggbupfeqo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gxhdiuoad.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/garkhqrdm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/grzxofvas.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gadbiszyt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gzsbnymwt.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gexffwgnm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gbocnjsgx.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gwporfbag.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gsbrvbzxz.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gsixicrpq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gpabcgrcj.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gkagdsktx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gjdbwyhuo.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gvhmtaouo.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gfbbqtoji.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gmmdwhhxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gasbwrbyz.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gwuvfeulz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gokyyeayl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gsfnyndtq.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gqdzfjyho.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdeqvdhvu.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gxtloxqyh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfpqvzwxw.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwkoigpkx.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gxycwvyiy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gecgpgiol.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gdlfwwnct.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gyjzsfjtl.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gigiwhelz.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/grimoiiem.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gnyhgflei.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/giwfbilmz.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghxxfkyom.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gqxpcgpzj.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/ghglklxyd.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gjbpfvfku.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gllwtdtgy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/grghrlfgz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gvynqxklx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gannwlmuw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gjcbcukth.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gvzojlfad.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gptqpxyue.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gwbwfyyew.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gciyngziy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gtjyjlwlj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gvsupvgwm.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gvhuqyqxn.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gnzgzviup.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gtvkiacfg.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gmovknnqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gxpfqbfch.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gmzsbfqvo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gjugzctin.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gjbobriey.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/ghvblhgnl.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gbjjctivf.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gmfjcrcst.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gxcgllyom.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gdjvvaddd.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gvafiydwz.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gssjuseab.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/ggqjdltex.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqjeznjzz.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/ghmxeetpw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gvrjndhky.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gbfbcfqkm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gqpqirlod.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/giaqvrrwq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/godbceasv.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gaiyttfdm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gjsegrfqq.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gumaxvygw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/grsxsylqh.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gllfvippq.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gueqbejbt.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/ghhspxqsb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gycfsefoz.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gwhxjsmmr.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gkokpzuck.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gzujdwsdi.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gpnkwlmtk.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gprczahfa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gcrdidvni.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gqchvqvnr.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gaulwgdoo.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gnnkvaont.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gudqrdwpe.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/ghmcxwcwk.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gslplgqts.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gewdexveu.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/glszedsjd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gybxettqf.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gcgxustuy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjdelwytt.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gmawazrxh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gtwgdrnmc.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gibmfxigi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gkvfytjzx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gvrdpfsvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmpbblizv.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gyqaojlnp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gjvdplqos.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gyxcveagb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gmumcmafe.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gpbbmnyxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gdvqgrabr.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gcdhwqfqc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/ghmpdiibv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gknoukmml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gedaotrap.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gjflsxfyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/genltdnxx.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gugogycis.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/ggjcgjpzu.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gavruvvnw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/ghhxyowbd.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gyuhvmfhr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gcvhbezly.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gqrbwizxh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gmurlyhqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gwloanzgv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/glfjtvspq.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtcwsigva.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gxvrtlhiz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gxgumoigy.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdnxlrjzd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gfbwwrcmz.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gdmlqbmkw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gbpepnxdc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/glrsyxvhq.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gusnwdjek.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gohopdnoa.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gdhjpkuoy.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gjupatyxr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gdkcvswon.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gymeijyti.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gnwtfannz.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gtswtujsz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gizehcact.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gxwlqxspl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gzqrjbdqv.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gsswpbfzo.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gbyddrkeq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/ggnijcpth.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gbzhyfdwh.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gvurigssp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gvftruijv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gwucxwrgq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gxlgvbprd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gupyvczuq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gcocjbkdc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gndsdjgdp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gatjhaqcl.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gcxvtssao.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/glviudqxl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/ggnyjtnqh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gnfvcgjfg.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gwvmdpkty.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/godgeqsfr.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gihiyupnt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gefprgvbd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gkuykpusf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gwazvbakj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gffznyhos.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gqczfoivz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gnpuvxzmf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gafuppdqy.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gileoijjh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gduwsdrab.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gtexiqhjs.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gqcgnupem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/grczgzqjc.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/glqdyixtx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gtrcxmnnv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gquaxnjzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/giwrxezbp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gizzneftd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gdlnsunbd.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gytfacjah.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/givflcgiq.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/glbafhutn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/garsuzwnh.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/geckposxd.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gieviptil.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/grcbcuccq.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gqxzprcil.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glanpvrvp.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gnhumtkky.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gipwdnmwf.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gixzskhan.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gxbsskutr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/goukszsor.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/goiwsnhkv.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gljuptmik.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gwkswuuvj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ghgxuoaxd.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gjgvqizcn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gdtzscwnh.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gptnqtpuq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwoxhvtzy.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gndlpqqhb.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gypintevd.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gpuatsdbm.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gybokbkfo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gumocmjmr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gpesdyabd.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gosayrtrf.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/ghnyglzur.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gtpwphnmy.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gcjuyzngk.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gimairzzi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gweoohjzi.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtvyirjoi.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gdjnkiskt.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gozdapfeh.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/grpnkiggo.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gouuffeac.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gqagxcmaq.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/ggkpcsjfl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gmddtdseb.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gchcozvfp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gudqavktl.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/grftejvyy.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gtgutwnnf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gnlxlkwdj.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gjgmwdbtx.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gylchdgvy.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gshyopyey.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gslcledtd.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gjtmlihge.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gykqnixtj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gjivwbicv.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/graysybvc.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/glaelkyre.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gfjsduzfg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gebjyyznm.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/ghmukxvbp.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gmdflisom.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gjnhudumi.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gnesexajz.sHtML


<!-- 参考信息 -->