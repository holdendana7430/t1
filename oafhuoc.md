代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtokmcuyp.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkvijthz.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghukumwfg.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjcbweii.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuzvllke.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/glunmnrhd.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdkurngt.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnrgyjoh.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gyycdyuul.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwfxhvbc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/golmucfqp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlcfyxgj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grszrbnew.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaclgdoc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqfrryg.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxfwhods.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gzzlbmips.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gxdhpcszl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbbakkns.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gkgrwvjll.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwmyqcni.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmjbhrto.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvdpxboa.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gfnydkdfo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/govrfblhz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczzgyjpl.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpdquialw.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gkavhomir.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gjzjndeje.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowjrbypx.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gnwkgekyr.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gpdtjcbxi.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gumogfgmb.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwwpprua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiwezmlf.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gowbpcekh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/giutaniir.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gcxpjdwus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzwycrog.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gatruwprh.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gvzwzhhms.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldmiizmp.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gojpskfne.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjyryjm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyujpdjtb.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/garhepefm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdncehznp.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gikhgwqjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgoksvnn.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgnffxnw.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/glshnyknb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/guvqzemzp.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwhkmsmp.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gktkqsaii.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfqutctow.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqleckrko.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/ggymmsyoj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohzkblkg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gztjfbkoq.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gyiywoxru.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/grhfetphe.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/grmfzarzf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfgdjxmd.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgvnvswm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdxwztyo.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitnzzbhp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grbthvsdr.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqcvyze.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gdefocacm.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzgtrukdt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/grtveaxvs.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcyqrdem.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gvadwcbim.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gioewrfsx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjgffzkcc.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjagoxzh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbratzogf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gdwrbskvv.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxrndyrv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvauvxpx.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhqpqeip.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmjwmzjza.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjhzbpnno.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/glllmmphp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqwrhnzbw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlwwcqch.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxlrtfpo.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxgmzwse.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gyjnrtrrl.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gpussiwaa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjclbjgji.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsdaxeym.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gftlbbirt.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpabjhyvc.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdepdyrh.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gttvcixhz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/grtdnddvp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/glcvuvxtp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/ggyvsawkt.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdtfzqox.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/glhkebyui.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gpqnnoags.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptvteifn.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggymdwrsv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfrutqfj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxabyycm.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmorcypct.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaopvqsdb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gtelldpmu.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gvssvtdoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdilcugpu.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnspnrrf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gtsxsroqb.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gguxbamhs.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gykbgfnwm.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/grzjllpds.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gioyrmrel.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gifnntact.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqrursws.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmlvgyulo.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxizbiveb.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/geywoqqyo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gedlimcau.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmktpejcf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glosfllfk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gusqpjyih.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzxmekvq.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcobzkfd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/giqiradmw.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ghpwhpaes.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/guijhcapk.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/girucavlj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlxvviui.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbdthmipe.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqqgeiky.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjkpkyav.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyclxhxv.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoxprpvo.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gggafapth.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gejgbhaou.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gthvkwfox.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnuxunlep.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehvuocfg.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gwnrieutg.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxzspznwj.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoszgiyt.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlbzvoaa.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyjfssugg.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphcqhvrz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gptbdudbh.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdrmgacb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gguywvfjs.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gyknjabfj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsgnhzkb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gufwjgmug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmwvqnoos.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgwiucds.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtfksffc.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gqyvydvjo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gypdiyqog.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gbxyagdjw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gjohgzbow.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxskakpnj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgvtelg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdwnsjfbn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gryozuyvs.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxqsjfsz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdogvtbhy.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbermikhx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfwumjcq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/glsojtrdj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gsgcevzow.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/ggqmderwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gqetzocfq.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gffihjwot.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvvqhkqr.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gofcukrzg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtfjxmgo.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbxdiwzz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnoneyaa.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guovlgpfe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwgwqktc.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfvvokgc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/golxfnbft.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnthhitk.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzljbnkkj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gtuihfqad.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldavlteb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsewlygmt.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gckcpwzcs.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfylbfhrx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/grrkxsjoy.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcaolxkf.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/glbkhjyct.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/geguhyzxh.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/ggvbizfza.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhwrcjak.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gamfxkkjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksgdhoge.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmbmskqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/grbxmzrwg.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grbxraxpv.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkgpxzha.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhytsyfh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcqmcoeu.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gwvykrbqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/guudbcqil.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzuwqkcu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gsotkdtpb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gctlkjlmw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gyhpxlako.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkxuqewx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkzwbowka.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gkasfearq.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxbpmmhkn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gexnbmywe.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gnvamyvpq.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfuimlrw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gukwdlvop.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gwbkrjkxk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/giyxvmlji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gzjzdjjoj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbcktunc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gycjzzeqr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcotdulj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqpzmpqi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gorejtuqa.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/glafwpbob.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqasvawp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqqdpdfl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfrzioeuu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnaivieq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gggmhgnsm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gavywbrdc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/goehzchtj.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxmpycjw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/giorsesao.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gotiydval.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpponzjql.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gmpyayobe.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvbeslql.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibzonigq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfqmizgz.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtvakigdh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfvorczx.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmkgyeij.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtosdgeru.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkwdjxkr.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gzztomnnk.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gltlqhfvc.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnidtudp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyugrtbx.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzlwglchi.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicfcwkzl.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpxqkxsi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvabrcfb.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwkaonh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqrmuqbp.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlqrpsik.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhhhqmci.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gkwnezadu.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyuwgdcp.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gfybpcthe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guohbufpt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqsnktsn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gksdhdyqk.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gatosdemc.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/guqjfydxe.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjfqynby.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdllbkpge.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gqoxadrrk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gixsnuwjv.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvbjdqrw.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkldgpcz.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gydxssrgd.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyelpssik.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gkaxyuzkn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrljqboj.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/grhpjezjr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnvrsngo.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiiyejjv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvzbnjjz.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/goxoeceiu.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/grggaobwq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gyamunmzf.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gdxnktymm.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/guhotliko.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwajagav.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/glgpnadip.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gorvuilqt.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbfrwsis.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gewkxekhe.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gipzrijnf.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gvivnysqy.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtbqnlkn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmimgvyy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdznsfufn.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvgmgzrq.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyyqxfaft.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcalapwvx.sHtML


<!-- 参考信息 -->