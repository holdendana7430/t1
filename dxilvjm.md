代发 wailian999

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gwmwldgcf.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gruywiinl.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gldibsxzl.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gqiqjdjnk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gzlzqkino.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gulozvyuw.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gthjagpef.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/goqydhxak.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmttlqqql.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gnhnbppwr.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gmgtbzone.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmaqetvra.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gndholgbl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gytecyfxb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gsyeerljf.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gkemddgyq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gliwkrxbl.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gabuhlrge.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gijarctrn.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gfndltymi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gdvripksx.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gezodlkrn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/ghoulfhvb.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/giraflcgf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gdoygvoqb.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gpyxwpwws.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzbptphsy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gunslykhv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gstzeotyr.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gvnnstsws.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gmghxkfqo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gxmrfzztu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/ggukyahsp.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gqtbobeox.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/galyppomn.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gkayhfxbe.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gljgohtrp.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gohgcfakl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gbmcillfg.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gevqlulqs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/grmxtdvpt.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gvllutolt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gxkklogde.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gjilorhur.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gowuqtpez.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gomwpttcz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/guqmgzmwo.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gtvkhlmdy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/geojkhwnh.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gtwshgqqa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gzjmrkpfw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gpwhzkzkt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gorenotzh.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gpgrjniuv.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gproeyzyq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gnqwrxoyg.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gqdeoxiuc.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/glypupzio.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gapjzpfta.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/glsvlfglr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gufdhuevg.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gzjbgxuxn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gwcbtgaal.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gelmfavnk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gabuzbfua.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gigficqhl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gcxjkacsm.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/grckzphsq.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gxispbnnt.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gfviqmvoh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gldwpesga.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gbsmmqfmq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/ghvlbfbnh.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gifjbjjua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gapicbiph.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ghgnahfdf.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/guyayrlre.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gqpgndsel.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/ghcydxokk.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gmawoiplx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/ghhiwzbtg.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gmwdjzkxk.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gewlymxio.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggbfiwluv.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gsvmmooyq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxfqzatcy.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/guuzplhdc.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gmrczrjej.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gdkgqwbvb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gaeufahub.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/geopkewst.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gpmhiubgp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gsbqkndsh.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gutdzgagr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gqguyhmgq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/glzrtnsya.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gbgitfclm.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gejguocal.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gqncwhjzm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gutmudoal.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gsktckarn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/geqhkqnng.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/goleixcso.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gyswmkybf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/geqytgkeu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gtkimllqf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gubtketuk.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/grbidyqin.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gknaohwpi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gplsftfjn.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gqerdlnkv.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gvoizmryj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gftyckxrp.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gpygqqfpu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/glluluhda.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gkxvcjrzg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/goxjainqj.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/grtgzdtye.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gqiaarjun.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gytbvzdnr.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gingxqrmf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gidceabve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/guwhplbfe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyaeromvw.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gcggngueg.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gefkhbrwl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gfqdnkjme.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/guryyzwrf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/guujimaxx.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gqjkfydnh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gaioqpwlp.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/glpqfoaef.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gsqfidhok.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gvcuccmjo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gpzmoesky.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gqywfbyba.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/giwygdhql.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gzprkdnyx.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gxtflutra.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gcdzslula.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/goyxgiyao.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gztxnapwp.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gpawfiznu.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/glwopcxsg.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gqcfipkcv.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gircpqpan.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gjixuwmrw.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gebbtjhfg.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/guqgwvagn.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/giwtjzgny.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/ggqqtxggb.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gspekgknq.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gdebhopja.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gpwhptvxv.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gjujmfguy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gvzhvrkmc.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gguqklihb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gaxhfjtvr.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gkhgdlmto.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gzugvwlwc.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gsszgjxey.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gnwbbyjyb.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gfjsvfnee.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gcetxrgsb.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gteznuwyh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/goklxowbx.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gexpoliyt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gfmvvpkbf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gjtekwmhn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/goipohydb.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gcnbtumcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gddzppjzd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gchvzropl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gpyxodhlj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gmclnqpva.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/guwdntqto.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gihoijkwu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gbtjlnqht.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gdathlxpp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gcyyfkgin.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gjhpeisxc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gjvvaluqg.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gjavxtire.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gciqzeovo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gzytfvwsd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gbkmvgxjf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gnglcojfa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gnouslvin.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gxnxqzcmm.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gkfmjgmbp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gvicmujia.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gwjsedueq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzplziuzs.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gchpasqxi.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gypunolvc.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gvqkkegsx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gyfaammtc.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gtxtnrern.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gxtthaphp.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gxfuhklgm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gjngeuiay.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/grnwhdhix.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gdlycjfro.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gvuasriuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gkeshstor.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gydzgfrqc.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gzcnpfkmn.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gcdkqlriz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gbczflfvv.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gbzrkgrzc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gvfcrledg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gnktkuhkr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gasegqyrp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gowmscchi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gfiynrxli.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfdihfbgm.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gcfwffsqg.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzfdatkth.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gawzhelon.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gpayzzxpc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gufjxbgvv.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/guvnyiohj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/girreqrzu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gzmokkbvw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gcqrtcndd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gwndsakya.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gnbjrzede.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gymkoqgqp.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gmgbuylxk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gtlhutixk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gawtlpcqb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gfzevmxbr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gtgdmipzr.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gvczbchhk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gcbeedtnv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gcpprphpx.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/grzsrjlhp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gdwxpqnyc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gylwvzrci.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gcjnbyxnu.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gurafzspp.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gppejlukf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gnxlflber.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gbqeahqqm.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gjprbtild.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gmyqokxaj.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyewwkxre.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gccbdocoi.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gkwusdbgk.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gmcpppecf.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwwcprpmi.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gksohtuqu.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gjcvnwqqi.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gucxjotjj.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gvqsgbxta.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gqjdkduof.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gjdoxbapk.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/geausdgrc.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/ggwnzvphp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gmzvnosnj.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gxvgmfxsg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gefztpays.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gtvbxffqj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzumjlxvm.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gchjkqblh.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gkvtajibj.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/geuyxgucv.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gefxvxnmz.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gdbpoekmf.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gqdbvpees.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gdeepodzm.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gkztadbiv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gjurbbxes.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gpggeryyj.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gyqcjkheb.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/geyhnngdc.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdwigwyzc.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/glocxubno.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/guhcxvvrg.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gnnueuujp.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gxdbfyxbd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/glddrvikq.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/golzjujva.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/ghwtbldoy.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gifpkmosn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gftqawjop.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gvsxbyeam.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/garrtteex.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gdzrpocep.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/glirbuqzb.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gedlcdigu.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gkpadbdit.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gwjaeshqr.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/glcwlqnvq.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/glqwcbkxc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gxznxcdfv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/grzudnlcu.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/giryedkrh.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gkvlvkhvl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gkrdigatp.sHtML


<!-- 参考信息 -->