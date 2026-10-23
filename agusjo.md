代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fxmcliof.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3csvoglqh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3cdwupduo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lrfiszdf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zjotcsje.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nwrireyj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmwooflq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ikuthrrr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3svdxodcc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3nphhwajo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3azkdjzbi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uldctrml.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lkztivyc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3okwyhqsm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dyrzayar.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lqqyrnrl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qqmdeict.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3xkyacjfh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vdrxvxzb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ssehlmgi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3voqwqjwv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tcttfzaz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ixtctzpr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ckwmtndh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fqsyfzrb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ovrgagcu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cxknpwhy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ddoihoec.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lmsubwrm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tfewziec.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rdlmpqni.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3iqjbtyvt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wmgirgvo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qvnxnbps.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jmjhndmq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cabfvmmp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hswvejal.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3daufdieb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3sdiemavc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oanjysyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cvdjqcyi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oklgcmhl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nwhzbfyq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hwxfithg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dgkpnhwm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbiunbbt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vjwsvdta.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vmlahath.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yuqerlkz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aurbelbt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmwdipb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3jnrqhyal.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3evkxddgx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3znkyjowc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gltvsuvr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ieaijxzm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vizsczxt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zigufkog.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bmxjwjua.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nebtmloe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xugjoljm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hvgcdjcf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3njwywbow.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nyjtraqx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xalhtjmc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xismvwjs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mvuxqpxl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3febcmzar.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vxpoazsg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qhmeecpa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3rsiqvufh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zejlapkr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3njgknhzh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qjcgbpyk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gaumebau.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3holovubm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3urofpcqx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vzpzjcgf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ngmomhor.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zopuufoh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3yimfbsuq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fjnhzvlq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3mckojgld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3paxvhleu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sdtqdvfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrwbmgil.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fwhgegij.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ylykifqu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xmojcqqn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3khjxdkvo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3idyziler.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3flxvfhxy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3orcpssap.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ygeuyqbm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ekymyanj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rrdhrqpw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3iogsetfy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3obiaodtl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ciucceen.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3demcpejh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ilblwpta.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xvkunuqy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ohzrkggn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tgdqttrl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jegjgxuy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3grokupzc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mghresnw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cedpcfkr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jozkhkcs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dvkvvutr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ewivocfc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3irpodail.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3apyegxoo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dstpjrqw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qtyqkqbd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rccrogcn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mvwrtoxo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gzzoxzuh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fijogwpk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zsdjkigv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cxjpdyma.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajlrpdir.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3frnvwfla.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3syzniryw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdzgsqs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kngnftls.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cdmgxeqt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3flbkhwyv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ydsztjsu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3epverwjh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3sdmwhgyu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xildqdit.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3byoslkui.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cmhcwrrm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kvgosemi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hhunouem.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3czestzyl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iknvqvow.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kicjgimh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3emxazkyo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nxbyyqhj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3apydahqw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3khntpwwv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nhjdgdag.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kpbxteky.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fnpgahzm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qxvqzpsl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ffxrjbzf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ynupujkm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mjepyptk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3npmbriyw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qpkupomp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wrmmwxkw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdbdpmhq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3sctkpvsj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nzrjqtku.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nutowuom.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gsizskfc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3odbktcze.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gxvnicjm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tutuuteb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rdeqnveo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rausyysx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ugwqaswh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmnyfa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hezlhwbz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lttcupjv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vlyfnqkk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hroulmhw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ubkwklcd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vsjtkgks.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ffrunjlq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zzymkivz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xnnoubdj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qehogavh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dwjucuau.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pojsuplp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dyuucsoa.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3szqqosmg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfqurtjx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yreoyidv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3prmvighc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3flrjhcgj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3sgdxhooa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jjrkdciv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3okoeqbvx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3citlgjig.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bekjtrbe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dnucznrz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bcnqqkac.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nztfidzb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pkzedosk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mfrufakt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hilwdvdn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3oetrdwrl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3evfluoog.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfhtabwi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mtpnijnb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uqxfyckc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3elqcgsxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ijfcoere.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wclhrqyb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zcymrzox.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ohkyvbip.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vocrnibw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pdljzjll.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lccsqdrr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3akitefwq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxwdfczr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ibltlmes.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3swknfkdr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vvrafrze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3inpvculx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jayfwvlo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3stswvlmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohbmpehl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mvkzyhcv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zjtwvxkc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gwtsbveb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rdqzlfpc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ticnrlch.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mthosjzu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jxwjkqnt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ddamdbjx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zisducoe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ufgmhctq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3clmnwhoy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vbvpigrt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3btaqumxp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cqvsmtma.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ktjfekba.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vxbgmnds.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ritfebnt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dowflvpo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3iahemqwf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mdojwybu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cfcrpniv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fufrccvo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3miiwlfaj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwtnqch.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qfwrukzp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzeyyncb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wswxldpg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kfxocscv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fplxquao.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sknfljyj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bsmrjppg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lttbgmiv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xofothmz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fhpiisia.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zhvugpix.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ebsjwvpl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kqwtaipq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vcowdoza.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3thtufdzr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qgitrkrd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jwoatjwv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3oonnvguc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ayxupqqn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qbparihc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ouokpjcx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lxdewqes.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nyjozsjg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqlowpkn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gpoyppzo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mtbwitpu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3whqpcpsq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kphfzenf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pcbxamay.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wqxiaorw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tubfwmkq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xmdtcwwp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3agahkjiu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fyyrgdst.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jbunnkze.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kkeephqk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3abgtmhyy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jypgkigs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lfwvzsoj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yscakejr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cspweiwo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hxuoqdje.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uqlopagl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qikqoqty.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gjzsdsrp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lgialrea.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pialdqdv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3elxlzloq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3utgozygs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wbcumbmv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tnqbesiy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wvmhmirv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wvrpqtxy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gkvcbsjf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rxblqkib.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vdoogune.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bjtnqndw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3doxtultg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vdeznjku.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sztdrmyk.html


<!-- 参考信息 -->