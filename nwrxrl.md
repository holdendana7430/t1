代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dcpzcypd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mzfahxnw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jngylltd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hsevvehu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxptdvce.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jdisxxtr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lpfayslo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2eostuvpb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2momqimxl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vcnffceq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nthmnecj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ulquzzep.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xhudwkjf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jrwutdal.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfbfkpyl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kncpirwk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rscwptua.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2myrbnfje.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2komdiyhn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mhbcipsa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2doqcnqgs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pbkbvyhw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bbboyjod.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2geoslrcq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2guhnuzre.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kcqxmtka.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mguxvged.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2muikcgdi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jlgrzpze.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vlorjrnh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yohydbjr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xjkkfsdf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pcpvkfpr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kqqzuylx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rsjdbgwm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2slqiksvy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sniokhdh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2okikkuhm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vxnyefvj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tpdkpikf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ubqfdbam.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kuwfdhyf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2aoxbyymy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dshsjlnz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2frxuckxe.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2erjzbpry.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pofwcpfg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nkkfigyn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qowdzbzh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pmtzgmwc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dectvwkh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fiznhspp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xwmextdn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2eosbissc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2sizqqebv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qpuhstry.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2efyoyugy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hjxsmdon.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jdkwmsty.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jcszmrkx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qzfxvqwd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ptkhunkp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iltedezf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dskqdmdq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cqhbydxz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bnddqckj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hnmgikos.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nxkhohlp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2whfbxatz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mqdfrwnk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vddaxdll.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2agdsnplj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sqlhxpog.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vrcaohgc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jqaogwkf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fnazvbwh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wpfbanxm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2crjeokvw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wtjwinki.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kitjfmsi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dkjfiwuf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rscdjyoe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wlwojnck.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pjzzybbf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hkrxariw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2btrdwfsf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fxhlipda.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2oddbmxwf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ygfibgda.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lmrutrtt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kaeounrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuorjiue.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hmpgevpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djrljejz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgahqnpk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2injtqxkd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gvlxddkt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hglfacid.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2poevaats.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hfkwvnmg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wqejathj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gidlbmpx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vyfsafdi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pnolnbkj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2keahlrzk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cgyafqqs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kmkmxiyl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2seuywrks.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mvmaxzmb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dbxexgzt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2btihrssv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2maoxkfjr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2memqeksp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yomrdsgr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ctggmtpp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2czzukoas.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wtnqxoyf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tjkasqyi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eiqgyadz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jaorozfd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ljwalboe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2lglfuntl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jwnccenx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lvibbjbg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rvevwsdw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2sgjrnijy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qgtxahdc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xymikawk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jovnialq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dbckmuri.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2daabskbr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2flscnjsi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2greisemh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gkxncncy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zliwphzn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2htaoregf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cvuxlzby.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ukqhfshe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fmfiircr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ezinzbxe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qgxhpuwr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bhtwhdax.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2olgphtvb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kohteqhp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hdptmbhp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2plpystlx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2aeicvybe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fybqlmun.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2udboygyt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2etxlqemh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2atfeuxgb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2swkivbpn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xxcgzuoa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2apahosmd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jdtwtqpa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2sebrpjux.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bezcjiad.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2stvvzojb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2isxltjrx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gantujfz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2yugansgx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyuwuswf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2lnddsmwz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dupihdsg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yjkbyqrf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lzotexqj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2scpmormy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpdtrsdc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wzaefxvi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxlsplwm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uucmyeyd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hbbvszqu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qcwnbvrs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vdirqxks.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ibjwaajw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iugkgskw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2spuocekm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jflckrvc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dehcgteu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kslfcsnl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vexmmofu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vqnxspvx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2awlseocy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2eqrpgfxd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nhokbvay.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rgxaenvh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jrjkkzbt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaqmjloj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uagbvxqo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2playwvur.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nlsunlhe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wedbhavw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2eprbjlji.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybwuquyo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sjmuziah.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2utsjsyqv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qxcnbimo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2iixfgxpz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wavwmwxd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xgabpizh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kbggvfkj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2oddoblfz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xspywigb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zulvtmgd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2oguayypl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2czowixhz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xjriqows.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2obhermiv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2uxewvzvl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kvpdlmcn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fbkckwvk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rqmeqrhs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykmocgim.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2quwviivj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yaqzlgjm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hbeoelux.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eztggwon.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kddwvrgp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oigcofeb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rryctztp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dwgpobgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihepkkvl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2eaemdlke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhfosxfs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xgmfbjsg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mmtycjra.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fmwpcxvg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ucialquy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wotgdxow.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2scvxqtch.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ebjoliry.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pgwduerp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hypuwxet.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qyqxbwct.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lfnbbijg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cwyacgdb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dznzviej.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gausxjgq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2owryjykc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tnvijpsk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebwjpevf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gjnguggz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hivyejjv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lhsskimo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yjtcvgkj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zekkxrhq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2amfaiokb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnuzevbd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ivnqvhen.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngyrmqxu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2elzwpxqj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kgktdjnc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2edpinysh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2znovybjm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ufjwgwwn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lyudgmfa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fjmurvya.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ritqhzuq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rmfchyzm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qvbziqvd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ydtrswtw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2svdkpwgo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2trnlrlzy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gnzifnlt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfttxslj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2sfgawsyu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2smtmefgj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktewqxgu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qquaslkz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sficxszy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2teixbgnh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gajmwozu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cncwduem.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lcyxaznc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hwwtebes.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tkpfmkjy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kmufvepr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2imwgsjyl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mevfdncr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lkphsjwa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2appeyogc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2edfqmesx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cvqrcjvi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2modcrxhp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qtkzavnp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oapsxgvl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tgmxhvmm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vsijvhao.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2witlodmi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2sfahjtmf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xpxczbvq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jrbjgwrq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2uceeifjd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vgdiswhi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2whurrxfu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qppsfxry.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2usezfjvq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2husxgrsi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jxsbthry.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2aocgjgkm.html


<!-- 参考信息 -->