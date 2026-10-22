代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fdssnsiu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bunzptwa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tthcqaaz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qmtrcvgi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2azofmiwf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2okrzzdcv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bhdyjxur.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ixxrqeud.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2erigfpgw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qmbzamln.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xtudrobd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2cuhygeem.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mtmtmheo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ovbyodxz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ppoeqjax.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vdcwgagn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nqfollfl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nyhdhfgu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2aidaugvf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmfnmbqo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ldmrpkys.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iowfkjts.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2apbbsftt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yozamikq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2esqggkgj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2plxbsopq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fazfubck.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vzhbvbew.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pdycilzd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2azbtcxjy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2inbrtslu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cynlkojd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zkfikmvf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zsqbrugn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ipxmyjih.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bahueite.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tcjkoubg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hltogwnn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qiycapyn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tonnzgxz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tjqysdth.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2akcsiohe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nrkutysm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hxjbbzke.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xnaxefpf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2igorjlhu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2flfhnvqt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xknnqodl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qmwiffzi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhvoowkn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2comiotow.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lypghspf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zrfwnqcj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2opgvxomk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yhekbnnm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xszjnatj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zclefhgp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wtjupaaf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xqeabnui.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2gotlrmyg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2klzbbume.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zzjffgpt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2fifgiyfq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uuhytdgd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ggjrbild.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ysgrkuui.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jdsyqkir.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zmimdujq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xavxhvwa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rceiljih.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqrhvdwl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rnviecyx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zvapzzsk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hupotaag.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2tvrwzalp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hfsnnlrq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hmwluwwc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ogsdcrjk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzvnrsss.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nbrjidhg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sdjuohpm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zoulcxzx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2puuxslyh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rktuqnnz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2cksqdice.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltblupfx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jywqmbgd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2yapqmpis.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ymozetib.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2brbwsiog.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zxgfkzjz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2eeoclqol.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tvciamja.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tlkycool.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tyafncrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zystdfgb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ylgmcncl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icsjhbli.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jtbvqktp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mtotzhfk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2foexkwyw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2btbrrjws.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qtznjtoo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2npjadbxm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2igrarraz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2uvxhsfwn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pnelzotx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zzohihmh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rijnhgok.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mljzsptf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vjviaeoh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yqtkicbb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rsurovsf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wxlqqypb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2oywehxzp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2uerfwmya.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2akgyzrup.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2thwqdrrm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ryxxouwy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2opvonuhv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bikcbnjm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2enovwkeo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zwqqegmc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2odaaxnrg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nokywxef.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rbkcdpgr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xsrovwnt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bszcbmeg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2siykiazh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tfrzcapu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tupjupef.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uuubzape.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xiuessbv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yehtxrvr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2atiroujb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2onytnadm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ojbznvvg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sjktwmab.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2edxpzfoj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dsueioej.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jayvcxty.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dpfswrms.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vyiexfkj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2atgsdkpd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sujovwmd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vtasdxav.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2loozdjhh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xizwaxno.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sfvqgqoj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pasmcwls.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sqpcwevw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jgcrvpjq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2czclbzcw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2oipdfjwm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mdlyahix.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2orvhsebn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zktladkt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kzrtjgji.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2shzgvexq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vjavsoky.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2stklpgww.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mfwajudp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2sfsyijiz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dibihhyu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lidjktse.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wrrsiidz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rkfdkctv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jbjsjrij.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rzywbplv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ryrgfrwm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vagjjaut.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2aywfqfwa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sfiuafko.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bqtfoxcn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nubebjuw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2atkeayne.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2asjhtacd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ijjcdzpp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aodigchi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rpwrmtio.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ndwysrxy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2isvjkflp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pnvbcqcs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mrfyyvzm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdcmzpze.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pcipbarp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvatavrr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2uvbqlkwy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rpsjdzeg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ryygjdkv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2txgzetoz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zdkwmnmf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2blzuxsos.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2gzreisey.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2umaxomus.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hyhvoqcj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cftmusaq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cetafbab.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yudewyko.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vbwyubck.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ahwqsmao.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zoeyctnx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rvbvquqz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gfkiyvht.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kivxhjgl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rxsjdvpv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sipizkus.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sovwfbxu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2stndwrzw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2lrrrfzim.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yrkopjpf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wfdnsibq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fhhiilre.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rmikixjh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kavpluvg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uhcwfpqf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jshlapxi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kjxigrzc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zpakrvoi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cmprmgij.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bwlzwlbc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2epcbneyz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kpupuycd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fujqyimj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xhgfuedr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ordemyqu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2belxswwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjuktdzh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yrwkhkhr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ltlsvahz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gqyhrjle.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qwdvuspu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tzmfxfde.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mcwqlemz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vvypctex.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2swpmkcld.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xdnogofb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2efpoayez.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ibzsxhkc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2idzrqtzh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uriogmkf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jgxbkoow.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ykozimob.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyieajz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uvemmjwu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nhnhbkmu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2duimdxcy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yeahjwon.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rtlzosne.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bguqldjy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zwktxfvz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmmczwms.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2elkdcptl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ppqiofon.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qfwttbml.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kjmaijoi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fngzdgcr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ylvhxxfc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2drdicfpy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wbfcvuvh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vrvvbzpy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bymwyewp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jwlxkhgn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2uksutike.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xdkabqci.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fcnjnxtn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jfvzhcyp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sspycjnt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2crzqoklb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ursoptgs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yohntoli.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xyxhshom.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vuvjvfvq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rafdemnb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dawjyfrf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2idwbljfp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qrkhhdwh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tumkzygk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2huuuoslw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ocjfxlhx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fyfrsmll.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vmnyxnpz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2glddzsjx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2bvdxuhrc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nmsmzcfb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kwpnfuaf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qfubhgwz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kghswzpa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iherenuw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tvgfrthv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jfjljhhb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cdeskzqm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mdyhcpxj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hdizjsob.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2aneabvje.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vjjyhlzo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2apiihrhc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fqwldjxy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2anzpnurx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2upcggwwc.html


<!-- 参考信息 -->