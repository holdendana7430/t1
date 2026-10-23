代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zotrvuls.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fltgtrzw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kirrzjyg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3swqdokdx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eevbaiyd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3oieybwrg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3doxewjci.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3noydinbk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ypfplqas.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3robzfjeh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jwxsdnim.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jjqtiayj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wemowtzf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lwphdvrh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tiqbykna.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vrbzgnlf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tkzhhwqs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ozfxokjm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qmqazslv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zvkqwhpw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ovccgmcw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rvbxejlx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xtfdwniq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3awgsyxfb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3quqoqvxv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3oadqncgd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ketqqpow.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3txefmgbj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qavmrvoh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vziwxkzr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqwcbhnr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ukjtoewo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iwjvunno.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hrgddxat.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3aagaozhi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fzpcaswp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pgxcnkiw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wwaapdwq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hbrunirh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qewbpzwe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3aetnkyig.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yxhndenx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qsvepnjg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ruodbipw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gqmnrrnh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hapoxprm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dmeeyvox.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3essbwolz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3afmnavgk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bfptvytp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mxbnhhpc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3heipztao.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3uitvjrju.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xbfozgwm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tzfheclb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3campcoup.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3udklepyk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vuhlceff.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrtzlsif.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3afjrbedf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gxgfjjtk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jdnavula.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3lfpfeugz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ozpbivcn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3affzmpbc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zynhdozj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dmbuazgw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fncxbexn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jwuaamly.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dusewizg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3beckrtxz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3usgopkex.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lfshbtgu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dryswadk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yaowwvha.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bpqnhwka.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3mvtweqfa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hhzapjee.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lnllspbz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hxtfnpcr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mtqerncf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hkmpqeup.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nnhitura.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syanrkiv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xmljhktw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feofobqk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cywpgauo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qwqdcjih.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3znffpygu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pvgaeswn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vdnpgbru.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zfepypug.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3alngsqof.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uyuswmdt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pzdljkfi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zupoamoy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsaajcdm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dqsciuqf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fqsybyew.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ltloisbn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tcowpahm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rhrppyww.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lbdlwbzm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3sofumnif.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pmtlfgbq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ynfxaydv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ltkwpkwh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3euijxnvp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ydrsxkqf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qhntuwxw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ihqxzysx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3parunqlk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sampyyry.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mszchlat.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lwlgmokc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eosojzum.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3epdmxguu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hmyemvop.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wynaezgy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3trcuqbud.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cucdhcbr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wtxsofjz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nauzvuld.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bgbfpfrz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fzybfrnd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nohyhptm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ybttjppk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nqugdhig.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dutyzizo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zybpzocz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xogvudiy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3apicakec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hrwpykqs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fqaaxdlb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3atprpnpt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uyxujmrd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tdbobqmi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xdnryqwu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rrcibnad.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dlcpatqj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3heccfefn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pwcwqqyj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bekcqbgg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ztoakeoz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ctrqdttt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gndzvifb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pcsfjdcy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nabnythl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nsdnzhpj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3uzhhviso.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qvahpnov.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ezvfmxea.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wpvuckwc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqhdghcm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3haxxhibj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3szrwyztp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jyxzwrea.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hgocpjsb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sukoscqc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wfrazgjp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dusazska.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gpcqaqdf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3braegsqo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zucyaguz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tynjxiyb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vwzqehmb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mgctmngt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3daokhvgw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wjtoqxkf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rhmoniav.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ggurtlub.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jhhducgs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ryknlyoy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3dwanhmwi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ggfyywje.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uvicwkts.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bjhuojfp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wkoiepxl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ksgoaokk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dfuwbytf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qxqssepx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oawdbcdv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ssnvdwrv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fimopquv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cecrtseo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xgiqpice.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgjixgtt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vnxpkdvp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qyynewfn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pndzhrul.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yynwrstm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3uqhktsmd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tjnsqork.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gmtpjivm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fvnmhtui.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dtgyxofd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxaazxco.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cbuxcptz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hhvhwceo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pnnocxrl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rdpojwsm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mgdiqctm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uwgniifh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dwlkcwji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfpsbwlp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3evpwgjnw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yfwwzckr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wssnghpv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3arknepjz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3doxwmhfs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mgqjkwqy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3neatfcyx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bfsfzbct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsdabfdp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ogoufzow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdrljhsb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zmbvtzoq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vftwvvuw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xycfpikb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3iygxakxi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ohfzyflc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xqcvmhtv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fpjnyqae.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yaztnxlc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tuyloubu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3evabivol.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pzonwlua.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xhofhjao.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xtjlurkp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nmrnvicn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bonbddmi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tevgjarx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3neglrmah.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fgxhvghe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3obqvwhdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xqnngaxi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hwsnatgm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3unnaknya.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3saifwigp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vqrjduen.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cppflphl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgknfmsy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3urdvmkot.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fexuyrdx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zznxizvc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gyjymono.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mvatbrno.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3efpejysu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xtcrmzro.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cgaoazxg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bybdpbji.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3enpmbcbs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sleoaqnw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jrjymiya.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3yhzsdhdf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjbcddo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xdaxqffv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sihfrbvg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hyixdqlg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oadwwqpv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3somamhhw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3csftplol.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ljclcsya.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xvbdnpru.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mnihbmyy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhuuwxw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wyupvjbl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lfkjharu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3aolliudz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wtmqxals.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nemevwyr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vqprwqny.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3twvvanhi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nkgtuqcw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qhcvubug.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lfpwaxym.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djqprqbb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gvhnvztm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bzpuilih.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3eisifiwt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bmugqfim.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ejspxmyp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ydurrltm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3syuodqoy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3uaxdkcdx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uooyvill.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3byrydjzx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qiywugjj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3sfcbhsow.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fiotdfgn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vbdjkprt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3satxjhoj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nsldtvos.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3eaauqknp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kurzmxvv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3szyimumz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3caymdaau.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jderoaha.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ebuetcxv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ozvdjfuj.html


<!-- 参考信息 -->