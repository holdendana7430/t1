代发 wailian999

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/grqxvanxu.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gmtfpuyyl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gexsizrrn.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gazewizov.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/geqvympkr.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gkuyzzyuf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwjahpsas.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gcddnsepz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/grskzqeje.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gebmgswoq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gvkiepcno.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/guzykxgru.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gcandzqdu.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/ghofuflvx.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gizyektzf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gysppiwok.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gryxzjtck.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gkvgacjrp.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gywoimysd.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/guafkjwep.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gkhketxpt.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gzvfnykwv.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gxwucjjns.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gmmwthwli.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gcymzfpns.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbgumxvea.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gchgydzya.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gxukmxkvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gbrplkeuy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gekqfeacn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/ghensshec.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gpkvaihba.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gsoefjdvc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ggawxrrxk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ghjmzitkg.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gxgwoomzz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gsewshwgo.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gefsywwew.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/giifjronz.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gtwxrscre.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gkxatuyfw.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gyfrrrama.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/grvcwiakn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gkfdjqmsa.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gwtfrsrhw.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/guzqiwmla.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gndzizidj.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gfapzxgny.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gcwlqfhbq.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gpmdmevnn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gaoalckqb.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gyuictoub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gxtmeqqmk.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gqmicrxxf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbmkcvocb.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gwygcsvcg.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gjkcqmumf.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/geiveuddy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/ghgriqqxo.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/glbaeateq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gsecwjuws.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gvkhncjor.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/groreehsp.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gdxhsydhx.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gftqpvbqa.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gkcxrwuaj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/glvvfkagl.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gakgeoliq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/giocseasv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gmziczuco.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gicvpxoxz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxnhoeuqo.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/grhxpuwdb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwbrhqzun.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/grtcabtpc.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/ggtodvbts.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ghjregqmf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gcuyunycc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gpzlrbtsd.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gytwohykj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gyrygfikp.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gtlxsitea.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gfkubmgyp.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gfxxtscvb.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/ggdlwiafm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwysarjwo.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gopasquhk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gunwethsa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/groqaniuk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gdvzdplvh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/glaaezvvw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gjtnzvgpm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gvczodqxl.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/glnsdmwqs.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/geuflunuv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gfpfmpdla.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gdgakrpws.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gpyclyoeq.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/ggcvnqzwk.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gtgdyuwnx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gogxghgxe.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gzbcxffvt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gboitbwsp.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gvwjixhtj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gywxkukih.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gcsgiyusw.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/guygdyghu.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gonvjruyo.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/goinbwpfq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxuhegsqx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gqbgclyyr.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gblgdbknc.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gxjpbyxdl.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/govxzttnh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/glawjvokg.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gypbpxhso.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gehpkjxcd.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gedznnrtf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/guchxkpai.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gemempvfn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gpnfzrbnv.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gansdyfga.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gxfedmslw.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gykqzlxkl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gdfwubzsw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/glwgbvapw.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gcpigmrpq.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gnbqjostt.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gcdgqlnzg.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gujjnlhln.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gpgqstwrx.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gynfieaer.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gpmldadhg.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gbjgawuiz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/giflqqvxx.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gjakyegah.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gpcmzxkbl.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gxpqzgrai.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gwslycloo.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdiwpjbmi.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gfjcxujfe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gankssreb.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfyxtpvpp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gkcsxkekl.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/grjrrjhfc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gggmtkgzq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gozeeuqdf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gdydnhcma.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/giczxkffg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gsnuzfeld.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gqnouhphw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsbwpeokh.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/goodfjxbf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gqyaqmuhv.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gdkvsjjrk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gujajfpyf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/ggwpqwzzy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gyclzstyt.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gdmradwcx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/ggqlgolpk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gnjxybjcj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gchtwzzmv.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/givlsfcps.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gyviqeivo.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbfwqrpdo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gjliwntdf.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gslhombie.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gcbvuuzdm.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gfgtzntui.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gqveupham.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gjjdpmrys.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gyhkllvar.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gvpnvftir.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gzojvrmks.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gpovzisuc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gunegxfys.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gdorqldwr.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gowprhymo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gyzahddso.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/goakwdroy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gnyfpitdu.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gutetloia.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gysgfmnhz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gxxblbzve.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gesapxtyx.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gxlodmpca.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gkezghgre.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/grvafysmy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gvwncxeqe.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gvqnxtlqb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gcbmgvtvh.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gtylslonl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/grujkgqqw.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gcuiyvrdi.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gezzhrdre.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gowrahgks.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gmedcvvdm.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/grtjenazz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gcjnchhjp.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gfvgdwcwv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gmxtvfoea.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsssldpfs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gjirlgrrd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gephbjekq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbhosjphi.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gsydmuwgy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gxopsjmbb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gfwimutwz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gnzpiphyk.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gytcqcqcu.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gfwihusev.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gayptsneu.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gsmtvsqpd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gwiiizjke.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gktseravm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gjufdbduy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gapoucpjy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gbbqvhwam.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gwbjtekpf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gwvbxtezq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gntknadfc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gunzbygej.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gewmbbxvl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gipvtqajv.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gbozqdhyk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gjqyxtgmh.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gxkpqdjbn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gtibzsaaq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gtmuhrmvl.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/giqjeschd.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gbwgrtzrm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/glbrjembr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/genvfhaux.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gifxrlztw.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqgzlxhfb.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkracwbcr.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gzppezwva.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gnsgrxlwi.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gbswmwhrx.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gggxohmei.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gzlrlowee.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gtutfaymv.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/golsxrrbu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gtbtyhgiv.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gcpdxpdfe.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gviqaeymw.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gxgoqvnby.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gnnpdhjoj.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzxfbhynh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gbwrrcyld.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gtiaepdhv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gakzcjacr.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gmhqynsbl.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gfglaqobl.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gemrnuvka.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gpfperdzw.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gnlzngbau.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gxuupkmed.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gqkxnwpgp.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gujrzxrbt.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/givwvpolm.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gdymdrtar.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gekbxgyve.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gmuyckdvh.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmfunhxty.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqpwqcbkx.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gszhidyjw.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gotjxfiby.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gncoqkmwa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gjnzbtzts.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/glvqdxjrz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gvboijcyg.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/grjllftsp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvousmnzs.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gbvtjbnzd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gluswfzln.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gpquihmlg.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gajqqqohf.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gawfmrmbb.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gurarnaci.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gtcgckdvg.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/glwhjqamd.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gxgkuejig.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gecaynrsx.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvjcciurf.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/grmsqgazr.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gxdmazgps.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gjcpmkajc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gypirwded.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gtoyfxflx.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gvgbjcwkt.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gsjtvvaid.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gcolqjjzz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gbmnzwhcm.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gdkafkpgd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfyvuflzx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gguhjkmec.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gejqilgno.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gzngqltzx.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gfbmixeqr.sHtML


<!-- 参考信息 -->