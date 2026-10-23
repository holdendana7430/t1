代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gyfrknga.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kpkjmsey.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ijfovbom.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rreslrvd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cdtowzmr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3tgxiwbwz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bdznngvm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3dheadsze.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ynngjjpu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yokyhzvk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ibjmtidr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nxzcdhin.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tzhqzbdy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tiohdzeg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zpgcykhn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3eibbglml.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mnytrcna.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kdnotioz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rnaptqgx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nvelmmvv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3avxpyeil.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hxdouffn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3uwdthmev.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xeyianyi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wudhyapb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pysyvljp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3xhfgqbrh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tyetqqmm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ssiokoio.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vciililb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3whmmgymu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kgsmywrs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ppkiutca.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vhpkvmgf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cnlsqrgd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3okicucpq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3neolodwb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ycnoyizn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rjmkprfi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3iypwtprk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vxptplbs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3eouatuby.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pyautuqo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ywcpdmnv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ydycemcx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3chwlknwr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3llurjwdj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cloxreav.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xgyorvzx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fhyirpbr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3miiuqwyi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cehsyjyw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3aljpltyf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zyflowpl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3njhcbtle.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ghezpbcd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qvwqrljv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qpswoonm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3khqudjtd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kjbdmsjg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ihfnauzn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cyixeizx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gvugicts.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qxyrvoqv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vpjlrqmk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uanbzbyx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3txtzdwoh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gfmewxci.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hsedqenb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zauhyiqb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qicvoffd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3iybjawop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ieheqxed.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ggiaiuae.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fqxysava.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lsksuymm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gecnvcrh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zjstcnmd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhaoskxl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qsuxwkfj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hquilsut.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3uuylvjve.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3efvamwfh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kcbkqhdi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ynkeokcu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gxtlffws.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ftzpzxip.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jjwipqss.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ummqwbxr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3whpvydps.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nxkduaef.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jxjazoir.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xmgqnwkv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bagmkzxu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3evgkspnj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hmiktevh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jcltypoy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kukjlcry.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rmxgbihp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3upksqlgy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lfmdwsev.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uqjsoveb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3mfnbmgiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhvexulu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nymriurt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqwcmwfd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3upsthvlz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wblxohsf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3igsikflc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pmtvcxar.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dqtrmxbj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hskpwbsj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3thxazunp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hauvfngc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uqdpfvcw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xdhxnrmx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mawnqyql.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vdfqkpdl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bjneqhbg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gldcbrbs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rnfsdmna.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xflpayed.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mlsnbbed.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3reavkcfg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3isbeahpz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3eepsrvzw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3jkrthfod.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdiunsui.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mfbdjggi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nanjbwzr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tqkdceri.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3sptqsqud.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fcmthydq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3djpxqiqb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3poclvnjp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lyvszvzj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zuhbnpgv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3neeckzxm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wtuldrig.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uapqsmnb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ogmhprxv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gpdddvnr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3epjhpeky.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uyigudod.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3veyvbrfb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3udnoqwwo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gahfltjz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tvrkhsqi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3leggjxpq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vlyvhrtu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3sioqdxsx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fdycxlbb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ebdrfwdn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wmzlywpk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bpoeyout.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bnhbkgzq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tkbqtgbm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ybelnjjt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3imhzubtk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dzsdhxkm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dzobfyvq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yrvhpjkk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xbercxis.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kfdonhph.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3aimexacp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpccohys.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3iagkbfll.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gxecsovr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ejmhjgid.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ksgzudva.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3yzzuhzql.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mojjzfsl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3uxfcgszw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zzjlduvu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqauhmkx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lxagvbve.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xrtbykad.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fhtxgymn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3afdfbvoz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvlkhuzd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tzqjbkmx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hhtjsbob.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lrgxgwhq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3honeykra.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zotfoggu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mmnutvjf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nskmkshd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dmzeiban.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ioocdiby.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ivhzvjnn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vkfnnnmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnstzwln.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3skvwzqky.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3imxvhfcy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uygjrzea.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yyiykajl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wqnvaeqo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rbsoelds.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yabviayw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eivwokac.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pekhhiof.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lrhuttqk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uqdsfzlj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qympxcsu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3spfaetkw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqbghzxh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3anuyrqws.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cegsfpza.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3omlwquvi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ufekglpw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xgehqdpb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hsycvxrp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hxpteawe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3curdiohl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jabvhspc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ajzelyna.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xdyedary.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pngzcqet.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjvwnjp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3aeabjqlm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tswurgpz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3itwnvtdw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kbzqhdck.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3aqethfua.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3djvczdse.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3nuszgyvo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xxyycxmy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3olhzxsnc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3twzaevhy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ygtcjrws.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wszpbpik.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hqhhvytn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uhovdctd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbmytiim.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pmwcccfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlwaprqt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nrtyhtrp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vhhjwvqc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ilrwevqw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iwypcrjx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vakdpjfq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3evossyzs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fztafazd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yqqggzed.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3reypfusp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3aztcarzw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mdifrvpr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqohwlpz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gmojzral.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vyxfkscm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3makmjjaa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hdfqzxto.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmlgtqhy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3sybfupep.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vpvjzxff.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bmbkzjuk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sxxzgnkp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mdtuumdk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3avgbrzqc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sysdsqda.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vdksywuk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nymwhzzw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mqjjieow.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zcgduvvu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kndvtbpc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zrvuxvoz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ersqzplh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wxyhcsmq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mxcpxeom.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zfcyywoe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tziqruic.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3roycxzny.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3leuzxcpm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vsretlvk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dnqzzjmm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zkibwqlu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iryswonf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mggdeoyp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nbaisifc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pkwesfxi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3orynaqnn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tmukuuxo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dmsgduzn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3esditrys.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wtrgqdbx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uzhxsnhf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fgpkuaxq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wmjljtoy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kjlyzrwi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fdwzeukg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jyjikltd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wrrcfqoq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ngskntxh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3knsfelpq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3robflrrl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zlzbqqzp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3orwxlskf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3glbgozxm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zltoowjk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3edszbzwk.html


<!-- 参考信息 -->