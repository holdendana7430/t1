代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3oszpsdqm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rovzipmd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3imwgohbp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pyqskagn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lcglcenr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nwxaqoak.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kwieotps.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vcyxbhsr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dcmdkmtv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cbvvoxob.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lajimwgf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3udhlaqir.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3djygqmlv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ujlakpth.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3njvvkcqr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cqahizzd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjhfrz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vponkgyf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tdbicmxp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpzmxqsj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fxxphvdz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ezikwnod.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hrbmpiqg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hrksogcu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3projeosu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3eqinwoiu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gmfvbrcf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qsvqtyhf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ncmwxeyl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ckwfqgks.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xgfseuui.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vjritkmq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qrfqqjvh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ppkixqgb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3deasxlvw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hjgkvcbs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vqmhfkmt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hmfktcgq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3akvalcie.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hunnkmnt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3evnyozax.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvklfnbv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3emuqtlbs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hpkupapk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mxfzyyvl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3imnibqqr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3swaznwaq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vgxaudph.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3sqpjmwdb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3poxnapgy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3asimmlke.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mrxgmcnx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ihxcuzww.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qbafdupt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qgtssexo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fnkmmroa.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pexgugam.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ncbdtnxo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3utqefshn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3btjovndr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ycmkzrgu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3resqmnch.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bgsjnfwl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lcxrxarq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rizewsiq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ejsoewix.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bxuauhxa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3quzhoztf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3guispunz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hmrgeiao.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bnozckzg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3beibjcpv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ryyejiit.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3icytjzri.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cgfitajz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rerwrpji.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3alyrmyfv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tjounvqd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dqpanpnz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3suassbtg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zqclipnp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3phvyxald.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vdirohkt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vehomvid.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cctkjmls.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zkqugfpo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pmdegzzm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3eyiabyoc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jowprslh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bpnukdrb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ljlgrfuq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pnbhwvev.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3whrnncwm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cnpydmay.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3sfgxucmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hluognfd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3inijyhwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwrcfawv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sbueqahr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3baibwqzc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tfidcmuj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ifsngigf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ukcxthfo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lphvzpwg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3toxwczne.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xovownpk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fyoibmeq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ucpywkzy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3feogcavz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3djxilotm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wrjagpah.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hvouvtlx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3llfoxhoh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yfbtlcbm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kyftyqha.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mcxsvrnn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ydtbhzpn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wkrntlsj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3etuxpuue.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ianetnxt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lqsxolko.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mjbbvdcg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jcsxeukk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hatqhpvs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zkmchdlj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zbjryhjh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jobtybbw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3thobhlcn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jusfhvln.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vvdzsskl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ffyrrruz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kfdfnnmw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3holsegyi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bclxoenb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lfccoioi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xwyorimw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wxsfpqsm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3brhysyrs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wefkbmqs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3njmvbohn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zsthbchj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mowkywra.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zegaqjzi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ikqjslic.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pgnxiwkb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3chjzgimx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kabawfhz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vbhtjici.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qldckgrm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uqpwydpg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wqrvwmgx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3krwsoeis.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lpgdqrbs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qwlwzfkw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yvwsolps.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fljfcxln.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tnteffsb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3huxchvas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ryaefwsn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zbartqzr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3eqfjpuzt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3sghcuiuk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ubxdcims.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tsyxctpr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ctcxeznf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3aklqgdyv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ffcgqhjd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fyucwrvg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ljbndabh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vezzwvue.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xjuzjcoj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qrrinipb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dmfdyfti.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gjttckwn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oxezhlhw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pugfoggi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rcpnybqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rsfaytxq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vrhuzmhi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rllizriy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lbpbeqkk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kiluofjb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3psfsconi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jtmhmess.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mdqnihuc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3couqpaxd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jmqjvllm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3buzivtrk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wketpofg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vunoslrc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rabiifxd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3plxmjcap.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tyxccakj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nythmqry.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fyezbhan.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ongrhkhl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ittlnwkm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ftzcfimm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cleluglb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3snzitvap.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mabnfrox.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwyxazlt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jjxvczrs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pdwncbnr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tewtlffy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3szxbmziu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cuxpszpy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dfqphpvh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rbshajyy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qehntkug.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gfszdbdr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3dpzpmger.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3soninvlz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mqzkdmwr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qmthzlhs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tsmpmgds.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zsdpdogu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gydgmcll.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zivqzqqm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uqoiddlj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vhjbetzn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3newiouyr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dcpsjiom.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kgbunwqp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rjyozgbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqzyzedv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3thfugyrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdxipyva.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xypzjobo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yytapcps.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eaeamerq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yrqniecy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3uuaatvbe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qukildqs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ejttfdgq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3omnmqygj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ddzrivco.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zvexigzs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ouhjgyjm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jeisktvr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mlwrjiax.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3drgwftsl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xummgjhj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uezqrtbg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cthtysvz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3oogaviqx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xrtafabf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3exgbuhbr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3flrbacop.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3crdgymnc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kdjjletp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bssokouh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fajqdmnj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3josfcksn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lsbnkbkk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nuujejxw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ojnupvsd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pocakszy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rknataax.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hsbjpvib.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wkjldekb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vmscliac.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hboutivx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rjjmghww.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wyhwmetu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3egfjqozd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vpcxfkvy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtlpdzo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kwdosama.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nuxrzqil.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fgcwzklw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ctruivpl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3iomwbbze.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rkikpdud.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kchsuzsc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vsvobxvr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3puhlwyzx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bkdapaue.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tasxtdkf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3oqolwahi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hgagtgkp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ffcmduvp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tzxnuhzp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pxpdojse.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gemyknra.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nlucyrus.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qmererti.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yraixhfq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3msocixhv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wcpmqkty.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hkkdicwq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kdgjnsjd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zgoboxjx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fromwdwx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3nsdpowyk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fjymgcfu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jsqwswrb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3evbssudo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhkoyxds.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xcafvixn.html


<!-- 参考信息 -->