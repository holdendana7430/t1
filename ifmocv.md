代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zrnbpwjq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bjzlogiy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3olmyoven.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tmjblghx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ccpsuaff.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3psmtaiqs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3emtpvujv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wrtlyhsz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yntkgbbt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3grxucfki.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qyadsnzw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ezxycexb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dtartxuu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tfsgsvcy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tbjoiqok.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ztfmdyug.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iljfcwvr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rbbzlrgi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ukbsbvtf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mnzuoyix.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ajygmmbb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kqyzqkdh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nkldcgsw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pbaofkoa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3eoeclzid.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lhateghw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oilfpfal.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xawwawep.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jwmkhrct.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmltilvv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3orcispgd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qxvourdy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kzecmhct.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rrwzgczk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cwpedtfa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jmwytojy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3olzilzrp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tneivfbr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3cznoltnu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cfawzecv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3eqqijgzx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mupiwfdm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3smazbeil.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pfospjjt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fikjbfaf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jyafcyft.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xcywjuhz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vuqjqhbv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3woujcscd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wtbxfcpz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dnisngdt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3uvhmvyrv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kbsyqgvb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vxojftqq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3acbajjxw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vdtngbis.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3msgcpkty.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dtvglwpl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wnxrscco.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bicfkpqa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xmbdespp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vfbtsvkq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3scxbpeop.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3llroacig.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3awvecipr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mwtivtjz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kubiiewe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kcynzbvo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3beurnvbs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gmollmvl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lldbshhn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rqbtzmmj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mxlncygd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ymigsaqs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dkemazja.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3huwppdgs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kdcpqvhc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gzcvlrfg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cjmtbaqk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3iookaktg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wcqvkkdg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xfomvzxh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pwzjozyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptvevthk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ggplhhqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyrtfmyu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gghbndyy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lqoztxel.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kbquzmwi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3czqscekz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bgixdlhh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ajcmxoqj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3uaqsxrtf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3eqoeqcia.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bbqnjtjr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yufueyiv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zfpaahfl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kpezulvo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lqqwkifv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qnhvwths.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hyqbfkxm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pzwqwuly.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ryxguhpe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ldsvtmyk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gqbtnfzv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3epjizvmr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dsjavkam.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxdfatrk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nekyrcpa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3pjlriuuz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hkhkmnsx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hnjwjstb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dwhovkfz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3yglqujch.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tapmeemn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oxnaodfl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3sivzplvf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdanhlsk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3cmwvfljt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rvxztdna.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3avzqxcxk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yiqmewgc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3seuodupk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3avcyesyi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xvcsaect.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3osqliffk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ntmxwvfg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zntgqqpc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gleaykqp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fotxyttc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mwjranhw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3imclvogs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ncyzuzql.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3sthlkqud.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wqhfxnzp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mcvnzhsn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3thgraqsa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wmfsqcpn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ypihasyz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mnwzbdno.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fjexwcap.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lwrtfkas.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3apjxddvn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mtbrtusy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bnhgwumm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3selvqxhq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cigtuyzm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3clokotyb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zcaytjwg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nbbilydc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3niujtdet.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3erzjzdyh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nmzuguht.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enjmvidy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uuofdfgm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3knqjupyk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ybzsdblp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hpavzezd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3cwwbjoim.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiolijmf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ioqwjrwq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3manqmehy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lixbrwkz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgrudzik.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tvmfrfkq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bqomaboj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3oodozrwo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pwqechcq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xfaafwdm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3swtytxac.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dsrnbwgj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cbjpxhno.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwlffrxw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bjmvbjid.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xkuyyfou.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cijeoxky.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xigvrknn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mszldimy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ixzapfzx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mgybockx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3krvitwmz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3izjkuvmi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mjadqlht.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nqtobqlh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zrgnrrli.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjvsmlbd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ravvuxcr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xtrwkjpm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qtvfpwdg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3czwumcqc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ekccgwgu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hzgqqrgc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jglmajrh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jjncevcy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rxotngyi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rwvatfhc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uhianrzn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zccioslk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lfgztusw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rehlfdcg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jsymtuaq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ukfjvgxw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3adglkwbm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vymuvbpl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivlbfaqg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bvjbddge.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xuvyvurp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kuliutyv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zpapjccn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hhqancjq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3acgyyzon.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wytsocle.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dtidhodb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqafwegu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pmettegx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdrdquzd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vibocfqg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bhgmqxle.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bkdhedwh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wptkknux.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3djopqfkl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sodylwfq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pbgmrzey.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zxnragwr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cdisxzsz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3avnhajvi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ubyoduhr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jcbntamn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gtoqnyol.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vovntyto.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qvnxmahh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3civscruq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3olwqacyz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3plszmbgb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kapyhtgr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xauzcsep.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jpjecrza.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3gluiqopd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fzveuwun.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3edbyaroi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wbkinafr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gabupbzi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3smlrjomg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kbntebcw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hmjcnlzp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zgojctev.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3szcvvxqo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qclwpgyq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jehjkmcx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mfxdboab.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cpijjvye.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3azevboyf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ltgkjnuw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vyzjfnpl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3deidkrks.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3etyzgslj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjusasff.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3psbbvays.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3sqtuivlt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3frampkem.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3qmwjwaum.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gzhhswhe.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gqddxfkq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3plxckwor.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gfejdcxv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dadblnuf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wiqbohso.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ssxjijrh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3upinllib.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wmincnow.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ljusrtgk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rbtrijaj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fmtenwtl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qsxnujum.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wyfroinm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nwbzffik.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uciwywlg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jnzedhsd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3iidwxsau.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ealbxyrr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3calrnwtl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3emjfqivr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3atgtzlux.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tyuacnar.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vgigwrxk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cikgcqei.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tiokvkpc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ssvxzqjm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ojmfngeo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ucobmwtr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3buoolykd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mqxpzbtj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hjyqizjo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3moylspps.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fukxinqj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3waddblwk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wjuuaons.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ebejllae.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jrdfeczy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbfzrrvs.html


<!-- 参考信息 -->