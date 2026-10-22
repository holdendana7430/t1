代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ogqwlzld.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2suyyrrqw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ckywlwzs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qjqbfmou.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iomjxojz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hcalbeeg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsnglczy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ypfvrkie.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2eqqgruwt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2quqqimko.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ygkdzzla.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kixgrqmr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gxzrqwvz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2osbqzziu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lsmndptq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dkadyzxd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcsohlbs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2nsorgcut.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lbnlruzy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2odyioojv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rxrpjthg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gemrrpzu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tzymaqhh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2iucxgnwo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rscvajcc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2anpxvqba.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nhuafrhs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyiqlray.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ydwmxmok.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wfubaqyo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eefpeulj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2aeecddxy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2djnjueki.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pvjdfhge.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lxmflbul.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mknpczkw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjuuvwzm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uwsfbjqa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hiezhgry.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2apgrdffr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kblslpxu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lltfufzm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aezkkxvx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ijlzgpol.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2evpshbib.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2krvpooqs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aqzktukw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gsgpjbuv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bngqarui.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2crgfrcpk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uphejcue.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2guldbrpm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ewpcvnus.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xhlinlsm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2pwhynihg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2npjdoxfx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kvymokxj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2igsbffzi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jplynykg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fcoborxj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2atlgjahe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qmlltbxn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ekindjjy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vlgytymj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2snukpzgp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tofqdbyj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jkzrvbwt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ftgutxol.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ypjiihia.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gmdjbgzp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dmgkjdgz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wczdhlsc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mbcoldxz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jsfvufgj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hafphkrl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tfgmaqqq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2shmgqyak.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gkbhbiqg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2querpjtb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2buluapus.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2sksbbufz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fptxgnei.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wqqxqnav.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ijvhwzka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zdirbibf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cyxutluw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dyhvldwb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wpbqgnqt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bdxjiblr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hwxoxuya.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ixehyltv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zegaqyxj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mnjjzwwu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2owqzjrrv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vozufvlx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jyrhvacl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pvamsdiy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dqwsvuhz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbgdufhe.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kzeqeuff.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zhacamwk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hrepsffp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dpabudfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyyvdnsi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fovaiczm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2deesynpx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uswchedw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2utqtbkvj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2grcgkpbz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nzqaqcaz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bjwufmzx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2turdmnur.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xqvltiom.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qsdeibqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xyfctreg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cdsbaqtw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aencehsd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rocghuwt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2etqixieu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2azwzhjyx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dttqewtg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hwowyxlo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2owsqtqws.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kqouqolt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ijlgjbdi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2neadelwr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pkfxyzeo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nccazqog.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2okvwmyoq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lgndgdjz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xpoeyikf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2prmjyqiz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qbdlgabk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2krvehsqv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ccnamdnc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wyppwvbq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qftlfjzs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ybwjestb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qhavleah.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hfegohat.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gyzjrzym.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zouyvjxw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lbgvabti.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ptruqrth.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ceoekfqx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vppwooml.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vvgftveq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oacpynbt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fuazfzuu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kbfwwiok.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ieslebjc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vxqrahiz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hgvfskpu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2htduwbwn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rcxexsuj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ssjxeqwl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kvryzykp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pshqhmmn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2sucjjupl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lxgoaelt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mevijoga.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ceuxofnl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ldvhqoci.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2joqpaqwy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dgaaovgk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qosfqowp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2olsfmgfj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gugqwbcq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wynnqixv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xeqwgipz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xhoyhvff.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2doyrwcdz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hcojhdzf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wgpexjet.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sdvdtyvg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zabkuijl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pkfgqryg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2etaznzod.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oabqehtk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcvxvttm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2darfsodg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2upypxnor.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jzuevpkl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zkrluyhr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2chdnlzoy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zkjwhhwo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2djqzvgjt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zrlqnell.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2erppcghk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2movvvexf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zpgmxkev.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zksiadsr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jmqkbbly.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ghxeggam.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jktpnerp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jxwabybz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fguvhong.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yrfsipac.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dfclnadh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xfzakbty.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rchxuxay.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2eyotjuye.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2yacvzsda.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sujporyi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymqnvlkj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkfvwth.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cskdwwoe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bzrzlglw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dpukyvfq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2glvrhfqx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nsgswivo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wattzduf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ivuhyxve.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lwcvjtsr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sbyempaz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ixblxjra.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyxdvgxv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2smqbprdo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jijfpljc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jykoxhuq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gpmrxlpl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zgdkdlca.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mpmjlavv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fbqjgiqb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jsmnhlth.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2uvvssrbi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dlbuswwj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xjnmpzkh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qehidran.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2txqgoirw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zeqxtmbg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2iustlbcg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nfhnmfih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejjxzart.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zoqflmse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtfteubi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wdvqdcmz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2heyjrjtp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2icwqqwib.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2srlyrfhz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kvagfgsz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uuzfwwmi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fzqgrrkw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2arerxndp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xckbxnum.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2moiqeknn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tofswqsy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sgvjvwov.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fuzejdjs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dfybccdi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cabgwfvs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwscsxq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2glvvpfvi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kecpbfsu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hlqzhxhf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hkixsvox.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wrtobmew.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2meyxlmmb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hcvlopxz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pyekqoek.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dmjysnpc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrkopig.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2frbecbdv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ezoytrns.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dxzuckhy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hhaprrff.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ypkvtwqh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zyauppsf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kjjewxqf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pkpujboy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2flywhfcs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zhqhpyqo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nfbmvomu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hlnnuwpe.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oxbjzqfx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2daisfqqe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ejcusbog.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dsiizhnw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ffrkwatw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2okourufx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cbvbhzaz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2aimafdiy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yvyjdpgo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kyftbjru.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2svpavcee.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tyticldc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rxjtxvmz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lhuyedqv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zpakpjob.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2timxnpgy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kdwtcmzp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2phkuiibd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zelbfgjf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jqrotxsp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yxtipvik.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kndvfoxw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vluidnuw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lyeawawj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gscbqfbp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kjrjawcu.html


<!-- 参考信息 -->