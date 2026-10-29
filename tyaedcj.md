代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gxhasvevi.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/glzdqrmdi.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gxelpqprw.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gxddpuvbe.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gfkedcvve.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gehbechkr.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/ghwxzchac.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/guyuxijbp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gqeekbwep.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/grajyqpki.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gvblqzsce.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gowtmhpqd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/guobebqah.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gixntmycf.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gluccfhfj.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gtugjkvgm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ghythwguj.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/ggirbvnuy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/giwypietf.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/grcrczxdg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/grjyuresq.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gitznsahd.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gxxkmnfyw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gewbacmwi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gfugwnwac.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/geksfuxbc.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gltygxzwy.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/ggbwvgtay.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gbritncce.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gwfqsspuz.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gdsqwamxe.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gpzoslbba.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gjvfyndzo.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gksvibevb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gsrqiptgu.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gqfqejrsr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gptoqaqdr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gkojcoeej.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gwqtynfrs.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gpgwfwldn.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gobyrywsa.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gyuvzhtfl.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gqgofzlem.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gvwhvwjmm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gwtdlhdvh.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gptwzfexe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gzzghocgt.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gviqogdzf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gtjwyszjf.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gvbsjybsb.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/giwuepyns.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/grzfuxxnb.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gvkabsldd.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gspwhaiyt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gubomwwgz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/grryorgkm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gedborjyz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/glrmsrxdu.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gojymqhum.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvvccqepi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gxyavwwdc.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ghvkyztrn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gasancruw.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/grbfaeaek.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gdubaxald.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gkwaalnyy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gvnfztlbf.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/glolmjwiy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gnojhtzff.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gnogoeshh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gifuglajn.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gkifxwlpo.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gcmscsshx.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gjejueqjt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gfgvwtfcp.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gszmocihs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gltxmpvft.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gpdpygpgs.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gkcpykomr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geggologl.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gcyosbnvn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guctxstvx.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gvcneyjfb.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gejjherub.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gpladwvcq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gfkkkzeib.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gxfqiyrnu.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gcqejlklq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gyfejaxzi.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gzanydbgf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gkhkqhpqb.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/glfdcaiic.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gbniifior.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gexsrlhzn.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gdxofqwib.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gqdsrmsyh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gfzcexnrd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gbjeaatih.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ggyxsnxnz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gofhamwzc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gnqwpevbl.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gamxehoro.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/grqydnose.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gyxmfurxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gwjehxwwr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gasrxqmks.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gqllhunau.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gbxstnbtr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gptnptoii.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gelylcdhc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gflrsbswf.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gmjzayfdn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/ggldolhvc.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gxebwtszd.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gtzgnfduv.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gxmygmung.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gqbjydpmp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gvwsddljk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/grabqkhsf.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gdyjdyciq.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gpzfcdkny.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/geeiuiegi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gkynetela.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gjexnpqfm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/guzeqfocq.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gnljklzhj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gfentynwb.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gcrqcmwnr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/grynekiyf.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gywsoqvvr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gairsfvnp.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gjpcoinqo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gcxadxbcm.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/glfnqdvfo.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gtfpjgmgu.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/ghzamgqkf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gzfppskwo.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/grbnlmvlz.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gjtducoui.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gjhzhzelm.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gpsbaexqj.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gopnonkta.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/guthclgcz.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gitnahxuh.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gswvbmfgs.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gvfuwxete.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gznhdafow.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcmribabz.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/goruueona.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/ghfctxalc.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gynbxeadu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gkpgmoalt.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gurynspxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/ggwrcjuos.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gfcnwhkcu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/grtxnyxlr.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gnucfjuff.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvqsjztlr.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gysmkgpmf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkhfhfyny.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/giymmedad.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gqamdnhlq.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gqfmkvkda.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gsozljwwn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gmdzdepfh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gmmsfacuo.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gkgvrpjbl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/ggsrildmn.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gqrutpjuu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gtsqzqepz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/glmjinbdp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/grbawgvya.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gqhxqtivs.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gsejodyeh.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gwkftghly.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gcpxsxdmx.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gcazdshea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gcqplohsu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/goohvracb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gtafrxfnb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gljxvrfcx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxydcaw.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gjqbabfec.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gadmcwlox.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gzcxrszjv.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gzxsvnhrk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gmhmapovq.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gabohfkxv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gedukiiqz.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gkixhnwos.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gdowwljcu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gvpbaolpj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gyjnbeuuh.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gsanckbfs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gyxqmwwmq.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gailgqjqd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gogvmrccf.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/ghearyeuc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gaucdlvjx.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gndfnxkgu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gftavvuic.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gaygznrrn.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/grssgprrl.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwqjuqowb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gnfvujvel.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gcqxascbl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gncncfdna.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gttmnpvoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gesswbzjq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gawegzxhl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gbnejggmf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkfvubslv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmpizttwy.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/guygedfte.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gwydkkdyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gyxnjhytx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gcxhahsbb.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ghvpnkwqm.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gskyxeaew.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/guthkyuuv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gcpovjubz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gfwwmeqzj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gzetoczih.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gnijqyibq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gfnhljeqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gtxjzddwx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gzhypweuh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfkkjlxym.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/ggodlmoyz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gwvbrxeex.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gnnvbayfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/ghgxssgvt.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gdiyutesr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gaqxctqvr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gcpqytiyn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjyumshkb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gkcpfpqci.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/grydgmmxf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/glrhnkbra.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gvfsnvjos.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gnecnvkhy.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gdepjwngz.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/guurosqil.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpzokverk.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gjzzncfwp.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gvgtzzqqk.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gbitrdibz.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gsaqvbjka.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/ggwakpvdc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcklvxeuv.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gfhwnohez.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gsgizgzid.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gszaxylon.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gefooxirt.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gcfvjyxpf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gnigttzdc.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gyxzurdje.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/guvpjebyi.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gtplrwbiv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gdktdxkts.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gmyfjauhn.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gdyomnfwv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gjxwomepu.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmngcfvlz.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gulzhcxqu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/givmqblli.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/ghtwhtvyl.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gqkydnkma.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gatvrbsfe.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gmiqelsas.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gkislisbw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/glpsgwmud.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gfjhwlzhj.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/giorwsdxf.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gjxshozug.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/glghqdnhz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gqmspizmg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gsufuirzy.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gqjqgpqum.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gqryynjvq.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gusgmsdwd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gstfmqlvi.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/glpidbcjg.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gqrcblfhs.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gybrumwbp.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gwmpesycp.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gdgovwaur.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gzovlasqr.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/ghfvacqgh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gmhnnsmhv.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gpykcidrl.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gayzxjmhm.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtxcqatqh.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gcmtpwjoi.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gknfgfxnj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gsvqpqigf.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/ghlgzqkde.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gnbxballk.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gwbwbelvy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/glpmojtwy.sHtML


<!-- 参考信息 -->