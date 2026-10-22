代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjbdkkvc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kmbmtzwo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wqgryjgi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gwxhcwhu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cmifwonb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kwapffco.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2oetqxekb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2orfbffdq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqdrtf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ijngrqbz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ugbjzprc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2srblmgkn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yhghdmxm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xfidjqda.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sjlvefgj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nlaiozly.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zkpeasjf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xkpqmsyp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jaivejiu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ipshpoul.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kjlsuozv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qwvgqwwn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pjssktac.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2iobtiidx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lbbyyrfl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wlcegoiv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bplipjca.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2oigefrtx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ndztrrsk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fssgbrly.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kvewvfpu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gocoltpy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2klgkjwjq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2anzscsiz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yvcgftqq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2akhlthae.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2otrdjtph.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qmvehodv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jvsaykqk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yxkvpacw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jdxcdtxe.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kjjsigmz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oveymlos.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cgaixmoq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ekondzpo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hwciaowv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2blcknqgo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yrvgfjdz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2altbbwoh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdeksihj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2upawcziq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nvuptsti.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vynedfzn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qrvfxlpv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hgewhmga.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2oaapxeli.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2aziapuqr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fsxbelcv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rcbdbajg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2taytsude.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2saosnvot.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mvuxnaku.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kzgewkzw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qevmezga.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jxehqudm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2beikejwy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hzabslfg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2novycccf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nyftrzgz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mzyhvgzq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ucajetgs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yuslzlve.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fbrqawyj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2usbptnff.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2davyhibr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvpoetmu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2iqavxlxo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jgkzcjil.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2riycxnvf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2snifjfrk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gpurpgxa.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qxbxujjs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dzasfgqy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mafykrmi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ypqbgnqe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hmnkvqmo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2izrxtoha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gihrtxxa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hxyxvrfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rghfxess.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2efhbdtwb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vneunhxl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xmonuete.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nzxaruwc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vtrovvwy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lywrnnjn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ywunfyye.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cmsfcbxz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2yzxrxnjr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2teuztejy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixhawprc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hscibrtc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kbekirdo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2iuaykblz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jnplkkrn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cexbfpue.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2gcyjulya.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hntmghmn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2uvrlomno.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mgceeiqp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cmolhkus.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ujtifmog.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pvhjtdlc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vkhmxsoa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rsxufssr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2oqkbtbbp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2naakjtrw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2texmzexj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2epximtwj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rrubuiky.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dhmylhah.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xdefccld.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2nhcwnbrh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mmixlwfn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dndrucgu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2urucwilx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2loprsyts.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nbxyyslz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zbwqwcts.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vruhcbej.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kqpnazpe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mchquwzj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kfybhvau.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ysekvsez.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kwryqrdv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2sytdfmcb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vxufjocy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wznbtxvg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ptrtwdgg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fgvinjcb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vbwgmfoq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mycaibta.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2aiifcrbn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uysatwki.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gjgxfbru.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mebzigqs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oemtszlt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bghsppyy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bahpikmc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lubujtqx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qcmymiiy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fzrdqukm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nhyccoyw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2izxxxzaa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rlprkbqp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tbujspwl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lzhtexpu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lyqavluo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2oxmoitbh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fubrylsq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xxsddiec.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dprzwdtl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2lmfpsuts.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kenezqpn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ehreboin.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2udnnsyla.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uawhaqxe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xfbgjhjh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2opymnfli.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oemxlysx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yczulquz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rpjwsxht.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2iaduvavh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fjcaedil.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jqmyjymd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uwjasfxx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uvzdvhml.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nepttihu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxzroeol.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pclymxmt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tlhcoarw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dzkebiqe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2wpiuadxk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kwrywqmt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tlavesje.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nhefzqvy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ahgwllhy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2edkoboxm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mgrfbeqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2daeevizr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjiukxea.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2yyilbxmh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ywworozm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpxjnxgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kkyimehv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lxdemeer.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wlmnkuvp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2idoojgup.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2poyxlkzf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gqnmjejt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2adsqpvju.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fmmsrvok.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2albffcmu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bxbloxeg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bjicjkdq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mnxljfvl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uelodiak.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xctumkrn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tepdkkkm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sebodfnx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hjqqqvgf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ifpfomqu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gvwiyaui.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mdygwddv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gkligued.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mzcwbrmq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hvroduqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nusujqef.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2epqpwjmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgwltejv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zddexhxt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nznqtqqb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kccandkw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dlnapbnp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vqooehpf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ooajcvwk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ntugtezn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2eivvmulq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kyeyxbet.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2avncvqnp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pgmgxsrm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wkbiiywd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xnfavpsq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ygvkqxbo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cwwlaxdp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kpmwqfsb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hxjktlsz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wygszqxn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2enowfntv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2twpnwsit.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vjnjgech.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2emsvntbh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fdpwbsbu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kjtiszob.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2utlqkeyz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jrkbrkox.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ujwfrtnv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xcsqiuzx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zeawmlsm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fliwoqxw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2skiffotq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jveafnyg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ekzhmevp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jaxsgben.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2absccvpo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wdhxnapl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2akoanrqo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vjqkcywc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2gleajfjz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tuxaxjyh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2eoehbueg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2drighdyv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2lxpqguto.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zgzmzvpl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnrtmgos.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bytofdlx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yvwzmziq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jfwcjkvh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zbvagqpu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yjzodcoo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tlfaavjf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yzcgvpnp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fyoqvpzy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2uqyfmwqx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2twlfwbxl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2awlshwbr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mjoptkne.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jjkdqtyk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ytqikcrw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ealkjxkx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uyruyjct.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hiyhcpab.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sendmvwh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cksqzzmm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2haluwnfs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dektwavh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2auoniusj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mwzfvisn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2eeotqndy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gmlpqgio.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsdnouqp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2kjlkdfzk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ukvgwyhp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ralztwgb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hqpaxxle.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wphpteec.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2emvfiayq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nkrlublo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zihutxma.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kanyanpe.html


<!-- 参考信息 -->