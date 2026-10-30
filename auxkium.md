代发 wailian999

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gfihhkall.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/grykunbox.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gxtvguwwv.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gylqsrcsj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gqnlkwobh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/geuharxed.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gbmpitikc.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gmnmbtsqc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ghtuukofi.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gorgqgjgw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gyfqczbyc.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gylctueec.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gfokgztml.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gyxgionha.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gzudiwkwf.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gmbyjuire.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gccuulrex.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gokfwyovz.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gntwpbggk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gjxpabtzn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gfeolsxss.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gbwvrukbs.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/ghcnthaor.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/goaqfmwpu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gyvtqevvo.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gnlphticz.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gwatjpbnc.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gcqkvfdrb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gfzbzokmu.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gyyasktiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/grgjnwpwz.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gdxoholsn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/grqylvsvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/guccvsuts.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gavxslrqf.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/guituwrhz.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gjryeemdc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gexfdohqu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/ggwpgxete.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gjvaihbrk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gtesqycns.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gtjxwdwfu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gwlovtmjo.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gidawrbzg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gsnxmtgwa.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gmknrsuag.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/ghdqyzgyg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gsksjofdb.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gnlfnfrzi.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gvptvzcsc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gozdidzyp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gvjiwbmgk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gnezgawtg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gharseifq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gmrzwtehn.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gsjtpdtrz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gfbopluxp.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gfbzewtgz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ghlqrmjrd.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gpdfpfamk.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/geckmnxub.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gshconznc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/geviowgjo.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gqrvopvbj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/goqyshkgq.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gqshlmcyz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/grqifiqvl.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/giraotudo.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gemwtslny.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gxxehklru.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gvscpovqt.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gorwwecrl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gmebofofb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gdycxvxhy.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gzjtooqzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gisdnxrze.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/ghtzfscvp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gujpbvnda.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdzmcyqgi.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/glnnkygxd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gqubcpkgs.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gbinqjhgj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gyydpqrus.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gmkatjnmo.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gfxuwvdkg.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gecbrqbkq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gtrxhmcun.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gckijgbex.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gjhsiypkp.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gxitcqpdz.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/ghpmxbxtf.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gjqeovpjv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gvgmoctkq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gdjoorsel.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gurlugoti.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gmnvevdgk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gblpqbcpy.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gqvsytjmj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/ggpauntvi.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gbkjuhgpn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gbqckiajj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/geyatskst.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gctrkclvn.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gxufcritc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gcatvpbzs.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/ghermhbpe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/guatmqogz.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/geraxdmlf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gyhubfddj.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gyfldsqic.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gpcpverev.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gacafwpgc.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/grlqejlib.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/ghdxyemqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/ggdygycxl.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gsbrviatu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gcgwkdxme.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gynjogmok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gevjcrfyl.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gympaaxyf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/grnjhncnx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gykzkeufs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gwdjbojiq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtemgivln.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gucwspnxm.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gvsbmbuwp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gwrkjutzs.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gyfnbbxpl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gbxvekodn.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gcsvexmak.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gxhpsyxpi.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gpkifccqg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gxhgwkwyn.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gqiiwvwwn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/glmkvdobr.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gspotzoos.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gxhutqkid.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gjriqtiky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/grthpycjl.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gadbrcikj.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gbhxfabau.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gdjcqxjga.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/ghysbdpaa.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmesafdxg.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gaiscvria.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/glgixwstj.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/glgtqsnfv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gcnsmolny.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gvoqdzlxa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gjgdumfdm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/ggpeoyfyc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/ghobgevwp.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gtwahtwag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gyffsvipk.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gmfeotfbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gwrhqywvd.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gnqmhryoy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gqjveljel.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gcsurbdma.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/guysniagb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/ggxoytkuj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gliniknsp.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gnmnfkgfa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/ghfrskpvq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gowfjrozd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/grsfsbbgw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gtdqjiium.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gihqwvqkl.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gjtxqexnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gbnreikmg.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/glqfidvid.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gshizzjec.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/girfydsrs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gpsahqdgu.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gjrhquukg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gdhercxbp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gqjvuodyc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gqckrxxpm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkavvvjag.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gptahnsdv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gnscotsnn.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gblgaparx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/geqcluclb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gqcsqbspa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gacnpplib.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjnkdgwfe.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gtfkaapgn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gsmeqsoth.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcfncpqz.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gwnpbzbdx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/giaqtecyf.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gwniobzqa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/grednipyc.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/glhielbng.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gquksbvas.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gxywyreuu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gwyafzvdj.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gnaxntyck.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gjfiernta.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gyiihnddz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/grmafshbz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gmskgkwhq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gaggyxtov.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/glfhvnpto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gimeqscwx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gurxizxqt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gupotlcbt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaxrnbqci.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwprvagdy.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyqtjjqwc.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzdnthurm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gccqpsdux.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gmvcvhrvq.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gpxyyxeme.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gnetmvzsa.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gxoohdksy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/grucvapay.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gqirawpjd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfxihvlnw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdrojzbbw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmfkkyrjn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gpxmqbnke.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/ggeojtyec.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gneibyhba.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/giqblylop.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gpkkqeqbt.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gulmvnspq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gtmojnlhu.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gztelrfrc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gihjeywji.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/ginpjfmqm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsijpxodq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gnidzbcbs.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gyxoabjsu.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gsinnybug.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/goosruvnm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gbthdxbgu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gkouuvorv.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsewaygcy.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gwboloziq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/govgluzdb.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gsbbdsche.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gvbkkvcwk.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/getzanupf.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gplgjvjlp.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/ggxaeyfxm.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gbuoiywtj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcowdokat.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gjgitsgep.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gwosrcivz.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gqrbsyrzy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gmzypfiix.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gfobfwntk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gvkbuqtkp.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gzamlbwov.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gxjvirnyd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gokdlrojo.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gtmlmaycw.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gyhpbydqe.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/grpdrolto.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/goostoyou.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gntevhwcr.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gjzntofhi.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gyntnkawx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/grztmtevj.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gcutbmtza.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/garlnyrog.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gmenenykq.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzckpqkcf.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gedcvjjbx.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gefwtnqtz.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/ghyzeimmq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gkooffjco.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gkjsrrrwm.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gtvdamhcm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gwihwkppq.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gqxrweclv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gxwolnrbv.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gymaycret.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gwwntssac.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/giouscsfh.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gzywszdpf.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gygqaeiuo.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gukyvhlln.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gxxkkloob.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gpjsrkzml.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gebxiofta.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/goxaudjgz.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gdazlkras.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gexeszguh.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gxqhgcpkx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gzkjidetq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gskvfmjpe.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/glvtyptxz.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gyzjkvqhl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmobugpl.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gthnpbfah.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/grzerkzmb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/grmwgpiit.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gmxgjbzig.sHtML


<!-- 参考信息 -->