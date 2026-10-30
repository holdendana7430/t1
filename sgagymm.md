代发 wailian999

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecnacotu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiqeqemw.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gocbghvdn.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbivwximf.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabddzmvy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwbuvhkm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/grafjgqpt.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssibscot.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkzkqssox.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gkixfmhbu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geezondmz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gweoiojnc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gjkfgpubt.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskkmipot.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/giytsduhe.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqngejdb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkzkaqjz.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gmiqnqynu.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxoiixe.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdnzbiah.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhqwmhme.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkuhbzupb.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqxliwbsf.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/grdfbvzpg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/grslnmvqr.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqjkthk.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gjjvoapti.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gbsyfnphz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdioxylwq.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gylkxubfi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmumyvzdv.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gkwviimkt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gzdftvccl.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gopmznmey.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gonqupcuv.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrpwjwcb.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/guahluurt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/genkmavos.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/guosdtsuy.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gnlyzxdwf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/geaulgxxe.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmswofexs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcsshrbw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljhembts.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfucwnhl.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqeqetmc.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gztppgkbx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gngryxlce.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gymcvlmbw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhxsrjuz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpchihas.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnydaxluh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/grbjlyhpq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gveduujyp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gbijqntrl.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gmcturepm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshbzczhs.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gytvzjeoe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgkinqyv.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymdzxamv.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/godmizzrg.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgrabesd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvaxrxfty.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjttkaai.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvgegcpe.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcvvvjqe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/grifoqkfk.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gfvedauxu.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gzbphjpxt.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwmmdgcm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjpevhqh.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gkunagxow.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/glaacqskk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gckusifbx.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/glqmrgbyx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gezngihdc.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gsqdhxhxm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhjbbsqg.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjavizdtj.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gzyzthlag.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwbbboplx.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gxvbbbcfo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwivgzbjm.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjqayjyc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gacegdsrn.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnyxnuvu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gicwjqcso.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvtsmcnz.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gctylvisl.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggnzeuvuv.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gepfumizm.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gyaafwugn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhregnuf.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gydkcxpda.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gomkdnuwj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/glvcpffti.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gusjavnjj.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/geuxcyzdb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gueyftzvo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gttfejwfo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlukrnef.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gppqnhvss.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqvbtuboz.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxdolvxvy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gojawynrw.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuqhxhoc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gxvuujhjx.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glyeisxrg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlztzqsx.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcyyhvqea.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpfpties.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwpjcdlm.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwtjeqyv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gueodkrff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gbuwhpswn.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkwixzktj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garneason.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcynndwlp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/geboxyxld.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwvvaekj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/goatfxoel.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gznzromuu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gemiuyqwd.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjatlzys.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvnhbbjw.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxqjgyy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ggfptqsqv.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gzmtkqsva.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbwzehbc.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuomvgnt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmthjmihi.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoqfrneq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyktijopd.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gceqgchxo.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymdmqjli.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwubocuuh.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdofkmoxa.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzxhbfdt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gewadpjgb.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/goxxipcpb.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfffirje.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwtisxcwb.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/godnblouc.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqncypab.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwidvqctd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqwpvfkvu.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdvyrfwo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitrjlmfj.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gmbfyfkmi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwhpmoka.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gnsoatyzh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/glwrabtmx.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdexotjtk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqxygcjn.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gtomeogdw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcjvinyjr.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyyxwlnx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmapmuut.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gijwbbdkw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlpxdqsz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmztntdum.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkmbvdag.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjahqrvp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gioogowpp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztrkmqhm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhkktbum.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsarbfzlr.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/ginhypqug.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/glyscddbv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gohpvfbuf.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/geofvgobk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsvdonom.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/guwqjqibj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgharnce.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjorvfpi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gszhetdiy.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoyvtjet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggokjygef.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrhukuoc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gvhhbrjij.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gazjahfum.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gprscdstm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gsvxsexnm.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gpklofzrm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gehbjtoiu.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ghrclqiqm.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gromcqfgh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbhexqay.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmjtcxxk.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gadtoecnf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjzuwct.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgcuysfn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gnlzvtwop.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gzktiznep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmhzranc.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/guwnaawxp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdmziviwo.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gniylylgg.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqksdader.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnukfqyds.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gikgersjk.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gwxcqhapq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gezidiysd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqsyfmeu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gsfoyqstv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugqxcci.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqjarvwd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/geobbyjrn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/giikkmtmc.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gxahbasje.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehvfocwe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlocvtdm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gyabwbusv.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnicpiue.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gsmfbpfmo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gptbgalvj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzhdisge.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/glyaupivh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtzwocjh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganofwqol.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxlikbrv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpykblpd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxeufnjq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gaszstzax.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzanayvgq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gjtqohstg.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/ginvoyqqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/goeqqirfz.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gebzopwie.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvrhysvp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/guyumxuuh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdspxwni.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaowwuez.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwupwgsy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnhmxksm.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gojczihbp.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmnshbfq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpruypfs.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbvmdpmmh.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gocpsegqd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdawfxefz.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnqwqczpu.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfxgtmdep.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gcgrskgrp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmlomges.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbvmqwta.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdnqhzvk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvywnhjt.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcptbakkf.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyvftdmc.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gpllcgzgv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcsdtifjb.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwhqbhhm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gvvnqwmut.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/guzzdnwov.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/goetejwps.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnimvqdi.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatetshhe.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjleqrcqi.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbsfjkyi.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqujniaj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjuokavmp.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztnrldtf.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gjdfpbhps.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiyfeiew.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gqpjjutvv.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/glbfmcfec.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gjpoawvvp.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ganjfjdeh.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gepplxqjd.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqqzcxjcj.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghabwcrrd.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/ghjxmwwhn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gcxuiyhuw.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gymhdzauj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gtsnuuiwq.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gieibdzlu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwmytntn.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guecjqfoc.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/glpayhagj.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/grsnwjwpw.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjmaimnam.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbfifwfg.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gexambwrf.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfgnoaewj.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjavavatg.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glptpdmib.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gristpgdl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcjtvpnm.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gefkvacjt.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gyswvcdlj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqdaovdh.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gguxjcpab.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gaczhvuoj.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/guqxaixyg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grsodyaxe.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoimnave.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gejyloond.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/glpobwgeb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjvizetis.sHtML


<!-- 参考信息 -->