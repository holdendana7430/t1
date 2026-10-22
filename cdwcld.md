代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mgjskzbm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uhyyjjhw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ckuyshuy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hjkcetwb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gxyndzcx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ublctspr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ytuhontv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycfxljvp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2txotpcku.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hwfepwwm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hdpxqhzq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vnmmnpsy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vgbthrjp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ntcnpvoc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ebmrymrc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tjcigxfm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plmubuhl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2paktsamn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ocdcgpbk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2icanmygn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hodxterf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2oazkvrun.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ygipigjv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xlgsojst.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jadqolln.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2sgmsptpl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2khclbhsz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qvwdvtqg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yttaiftc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2njspemxh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2chkxdhdx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jscjpjas.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cuojtrmm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lreeqeiu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rbdklgdi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lzlficaz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xbathmga.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2pbjuxsjc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2weptzwaf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tjgiunjb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xfbpubdy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2titfduiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hmnmvfbc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ojapcxsi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jbkeigji.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugfbitfp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pwwewrkm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2aqaaerno.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lnkznbbh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2aqgjdiiv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2grllvvgq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vikfkzvk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fvfjlbtn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2veybfmnd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gfzsbkan.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wkimcxxl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2sjifbjev.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qxctgzsz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ajoahgab.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fgtuyjge.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2aygijrkc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2nyovcrih.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2etmwwaur.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xhuuckkj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2shpfqfad.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nmgjzgor.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dswqgohy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qolkxmsk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vrwdyseu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ndwojawq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ggqiozxb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2saeqodxi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yatnywqj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vecxclug.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2clpnitpd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2phloxlqr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2olucjder.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dhcurnas.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rgrvgzli.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hilyevgd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rrebleba.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tgbxpllj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bpnjtivi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stjzpuxu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nqfrfiid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtobmjqj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uuahzyuu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vzfeziov.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ftvpoift.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uultsrkx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nkxfcubc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zddbnjws.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uhsluahn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bzttutyd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hcqkwpyv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ymzpbngt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rffxidin.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2poltyfnt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ipemtoho.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yooujegr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uhwhsqun.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2crzqelho.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2regtqscl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2udnydpyd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bsnxsvvs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jemnnhnk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lsgsxkpm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yrgmmres.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2iyftrabw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yonjggby.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vuglfvur.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsbieexg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2izpylqxf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2yanfkxzi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ofpketbu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ynniquak.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2evhmewxc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tqlfhphc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lzqimuto.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2glsrkaju.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qaoxibqi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2agvweupe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xkzzrjsd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vvxsfuve.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jmxoyxjg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hwzdmkqf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqblyhx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kuglwghb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qkukpuhq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wedqugqc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hkynlsvp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2piaccxtp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2oqsryyil.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qcpdyzdq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2okxrzpcx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tvlcpukn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hasushqr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qjwmhwfm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yhkwjayw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gggtzwxv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2clxkuozc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tbsyqkvp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bkkvhupl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uwthsrql.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xmljrtpj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2pafxllut.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2eoaljtxs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wvvsliex.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ydhqdoak.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mdqwxawt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mtffbama.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ncdktpzz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ycftxxuz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mchshcgu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fmdnrcsn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2goihnvcj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2zclcclqy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xtzqhrsm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2renaqnak.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lenstvie.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mjozqykr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2umbpvghm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ddhhhwws.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fubbisaj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bseyhxql.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gkqimika.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xuyvoneu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wskzvyiy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yoezxpxa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2etpkgbif.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ljvhcltf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nffdckav.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qjxfrlqd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zfuwemgt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2iffelbwn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qkbtkpbn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sorzipua.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2imheawyc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xmekghbt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2icrrnhst.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xjzaystp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jxkdkvep.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pxnshuym.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kmmzcniz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2toplswlw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dniwserc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rwiydker.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lnhxwikt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fhmkuxbh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xrqgbmdl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cbfgpfeh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kxukbohx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mswzqgpu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ttnrvgzi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wwesuahb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2uaninjtm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2owmiqivv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hswwszxi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2actalryr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2btzqvgzp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sivphkkh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qrbcmpfj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2umbwfkfi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ugwlohya.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zpgggvzc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bllzsgxz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kbjllipo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yxlbhuuh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cpblqkmb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gtcehtrt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wtypjqef.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2knzectba.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ecttgqzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuytwcua.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tazzecsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdqzxehz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2twoxctww.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dcjjgqld.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yaaodjdd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lpykdcgk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qqgmhhns.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fypgaqmj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cfkyghaz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xhrpbmsu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hsxwmkcv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cokkaznw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lkhazzkb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xhukitzw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wvlpcseu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sqrtwjqf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vqwhnbvg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pwepysqz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ickobjob.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cqwuxbei.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rvgqvfua.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gdyapmsw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gqehzydg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fksyqtws.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qciabhlg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvrgqhnv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yqmqaoss.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkxrpqo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2acwcpqjq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zhmdwbpv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vtiahiwo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2iqvmfsgm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zrfwuhqw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pwfktemj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fqjrhexx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tjfarxel.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ccwusapx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ebpwdiaw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mwkriagt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gjngktix.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tzwckrfr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2rgwmghti.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jmfetbyx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nolxbdgq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2cbyinfip.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ogvgvjin.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hmqgjgss.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2grozscai.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tborqlvs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yxfcjsbi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dvnkssbq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmyytth.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2quntvmcg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hakdgrnf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ioaugonh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2iyczlalu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hmzzydul.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lgyqpgav.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xmnoctaw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ibacmhte.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bnrhfffd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vzaprztk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xqxhinix.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wemsjpnu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2mnuzdujt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cuksdvgt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2grfhpcvd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2degjeeuv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vkojvoac.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ccnepwev.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2watjknfv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsvrnkhe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cqayzlwu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lqcyhskr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2goodolie.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2llsvglzk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2himwkjif.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2borrqcqc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wsxxowhd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ozaxrnff.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2iiodhknc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yppycnng.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mgqpkjef.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lskjlwcs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ddiqcemn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2auhixjoz.html


<!-- 参考信息 -->