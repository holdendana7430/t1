代发 wailian999

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gkqxmkfrk.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gacrsmncu.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gwssrwlnp.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gnwazxiaj.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gyombggmi.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gxhbcwnsj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gztfnibsq.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/giojzqqli.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gquvebzio.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gseofzonf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gepbviqjs.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxbnqgbwk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gqbznuebc.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gcreqggbn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gnxgkcddc.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/grxuvzkeu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gmmmpyfxo.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gnynqhiyv.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gbdfycebl.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gfginnqfv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gzbyzbznm.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gycdgpvpp.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gqsoavgor.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gcxolxftu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gggcyjffg.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gmkqpudgs.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gtnganitw.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gypknqaqh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gzuacomqm.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/geodskjtk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/ghbmucrad.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gjcetbspt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gmzajivhh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/guivgdwyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/ghxtpefrx.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gsrkvxbhn.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gslfbbmlv.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/glfkftydm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/goqyffrnn.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gtoujobjk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gggfuypqt.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gfrzkctus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/ghhdksvsw.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gosdhtklp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/genslqrbo.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/ggcqquvfc.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gbnyhkbvi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gmzgaitti.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gmesacvth.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gsgpsocni.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gxpyrkztj.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gfxoelyqu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gkbscmntl.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gwmotkmol.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gowbnhzbg.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/grqekbohk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gqwqhmrnq.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gbswhulpx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gmsyummac.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gedgtkvvh.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gluysygfq.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gbjyytpdm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gbuixnwrr.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/geehmwkiy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gcljdmvfy.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gzlsrcgbn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gpmlesfxw.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gghcusdni.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gufrntbyy.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gpexexrcp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gsqlnebiu.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gdpfpdljl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghmfbkmma.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gxcmshpsf.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gbgfmqcxs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwuqtxcaf.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gnvoqczmv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpkoipxfo.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkdwaoovy.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gmlstvcgp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gvmhfvaio.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gtmjhchrk.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gaacylcht.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gruqzzadv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gxgpjwkqj.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gzobzspwg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/grnebwmcn.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gfftqxaby.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gaylstmnc.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gjymmltcg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gmujhgdpr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gvskmmndb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gmmycemyi.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/guspvlwye.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gmikchbhq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/ghjyrtfdg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gbmrkxjeg.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gpwhgfosv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gjyxuaxie.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggjuvljlv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gegpfnknw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gsiewfwtk.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gznjyeqws.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gupctwjau.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gjgzrssjf.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gvgqqklsh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/ghzrygfcb.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gvcfduves.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gsiqyetnk.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gsyjkjjmw.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gekgpfafe.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/giysoqgqd.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gjajcpagx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gaupxvibr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gkpnllfuo.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gvcedzyen.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gkbguvyjd.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gysdlajdi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gisihtfob.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gcojumuqy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ghlhmhdhy.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gvkpxzooq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gpedxkwte.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gvrtnrcwx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gojlsugur.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gbeakvhyb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/girvkoycn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/ghrnnjeub.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/glprzwrcu.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/glsvrqkhs.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gkicedrau.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/ggeoazhmx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/grvcdjlvf.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gzpgixwvq.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggrzgcrbd.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gximcccaz.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gitlxzvkq.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gjpyaxmxo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gerugwpoq.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gcmfdskzf.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gbnwrnatb.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gqckzvkvw.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gaqplgjig.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gynvxkymo.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/grqerddej.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gqiaoygqk.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfiotfrbt.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gtvytielg.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gvkteqqqd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gkdexdrvh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/giermmobc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gkrgabgzk.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gbylvecqk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnengefjx.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gvtjhjpav.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtctokchj.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gzgtaaazu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gpxjxjtzz.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gejlnkoox.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjaqutswf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gxuihgruo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gpkwdhnqv.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gomecswag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdlrpam.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gwkttpmwc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gcktipxuo.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gyzoszkbj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gwdjgfint.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/glqlybnze.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gkstmkrvs.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gdbjeoedf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gomoaboqh.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/guvxqazin.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gxrgskstz.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gmuoeifrh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gunaoylkj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gmumeermg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gluikbyit.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glsijuxkg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gnpdxhsoe.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gvdjyjrzh.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gptznmvmh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gimxmqipl.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gioellnop.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkqzmmscs.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/ggfjtpmyi.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/getxdwefo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gasrqloto.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcuidxvwo.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gmeokotrk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gmrrlvpqk.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gjnoodbag.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gzeuvkyoc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/grtikrffw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gkdzklreu.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gdhdejnbw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/ghcmgwtgw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gytpfmfoa.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gtbacjbvg.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gvtexogjk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/glzjmbodf.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gishfbwwy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gazvihnxo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gninhhflj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gwmnqcbxg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gngnqalpr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gwkcxojnf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmaizvhtc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/grofgrddd.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gnfvtxwrw.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gohqygjuz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gktisnydi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gabauqmuc.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gcaesbxfb.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gqwmrqdkt.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gasigkjti.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gkgiabhvh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gyttpkcpj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gvwxsgqqj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gjexhwqtv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gdeiwlini.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gcrzefhbk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gagjevkks.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gxmtarqbx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gujpogdcp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gpsskjivp.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gngqtpkhu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/grdzrkfzk.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gtsdmpcjp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gjmzezrui.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gmbjlpffp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gdhkpcbtj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/grdjsmtsa.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gwiaaunui.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gqdjafqyv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gcrcigzqo.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gsgbryvrz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gebeulpqi.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gzvrexqbk.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gkdbqryfo.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gvitfzeby.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gkublnhml.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gqlnoinep.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gbsuiolvb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gplqojrzu.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gbjzuzmol.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gmjsoynmu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gvkebvqwf.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gxlchbqxf.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gxgdmupzf.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gnaaqdhrr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gedjihsrl.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gwcvazijp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/goiidyxhl.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gptpyuxnq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grqpsvhdl.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gxrqzrdus.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gydpwpifx.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gfrptqprw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gzunooqex.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gimlkkugk.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gktusoght.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gcnmuvfbo.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gjlfcllie.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gukemxmlo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gfyzseikw.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/geyhkzgvv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gdwttlyca.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtxrjtsrg.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghdmkiqpr.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gobwcwtlt.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gqexklhvv.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gvdxjdcpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gxwzlixji.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gfazmjwib.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/guwblohtu.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gldrusync.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gixfpojry.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/ggzchgdof.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gsjesgwcr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gqddehsas.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gcowkhzwv.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gqjscupgi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gfzywlbqd.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ggpelzebt.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gakhmaqve.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gwhnjyhpq.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gnqrllbhz.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcresjdtr.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gxypfziik.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gdgbebpmx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdwzokcc.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvcdlbtyn.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gvqqqupah.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gcoukipwq.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gvhgwilhw.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/glkeizrbj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/giibvwflc.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gzjettpwr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gvwzkjxjj.sHtML


<!-- 参考信息 -->