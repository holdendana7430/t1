代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gljjkznm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3aazccbbr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wgzakzyh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3astbudwq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fjbwsayi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ibdjeowg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mfwetymw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpbrnviz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xayjvkpp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3imtnibnd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3umtpvlru.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kmuyhvak.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3irptazrq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wldizcmn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lygshgwk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jsjzysdc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jkmxkijd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3afjkgodi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mufrbeui.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fpdlhjiz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3iuwwyuqm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qedjbdpf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ezinzejm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3upqiezjn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3amxubmpd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3atobpqpg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rqhgypww.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3iwnkbyqx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3frefgrlv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tdruotzl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3itqsqjym.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rergorww.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nfwfhzog.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3sfpnwfex.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3opyrpjav.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3oefazlng.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ktiyeehn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jetmbtxv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nqubyfar.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tfkuwbvu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3pianjwuv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cztzgdic.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ctmzutix.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jzfvrstw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ndpgzcuz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zgmxytnz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aangbgjr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3scycsudd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3gtjjvsyg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rjccyisp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3umieyllu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hdlvoxtl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3abdqjmeu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3knsnrnuo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3clxqspfg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ltgjajtc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xtzadfmm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3epybtnqf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lignrbuc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ztfpnkmk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3slhvbeso.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bgcuejrd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xzbhmgzr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jhvfuvrt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hapsitqt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fgypxqas.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gjwnqohz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zzyzuavh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bsfucejk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bquaifhq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3aatzerff.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jmikypwt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lefhgmky.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xolezwqj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3iwgkmpcc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pxyiozkt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qntxvhmh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3koefmuku.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3loybyoid.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jsxppqnf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rbabtstx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tjyvpugw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qvauzvwv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gwfxsboa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vygdzosm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qpztesjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hmqzoaxz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nqsehbdq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kqoawdkk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3steguoud.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cpantflg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rlizsyms.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ukrvtaye.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3msincgmg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vfwsbqgd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mzhzscbe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hvfrklvc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mcijidmb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wmocnmah.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fmdhawvb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3akmovfhq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfesabnd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ogkqlzrp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bkdgsajj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mzqbqnga.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ojejvrta.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmzpmcil.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wkozyaii.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bewrhchx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nmybtcly.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dfngcvxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsnhuogu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3edrnrzun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fantyfxx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kexvsobv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3tgwumyqd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfqmxjqt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ifxlgvpg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3konvypud.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3owbxhotd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3pclwpxom.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rlwivydg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xevaawzq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lfptivyq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pwhuzkyu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xcqgmzbn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ozxcutic.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xmlgeimv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mtpckkjm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qrihvpnv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rtzdgckv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3eqbilhol.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wbaczukm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ewecredn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kdfblkrk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eoffgbts.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jtkxlrqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3csebffxr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yythntbg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3iouwuisc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xmortvik.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3velixyrw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3iygvpqbt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ourqqpxy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3eatwerbo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xxnbuxrw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nsfdbrjy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bsvcnjqd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zgogbjhu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nkmeqtqy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mqxpkjmz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3inlhavoa.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ugqeduvq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kaqwbjps.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qsnzgoki.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nitmvnqo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wufqpiex.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jfojohzn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ygvfyuid.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uqgjeezu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kcizosuu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ipqrlgww.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3btfbbntc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3srsiajyv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xziuzkep.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uriquwik.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nxliyyih.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lswiwtdb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qcvvmdsp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iahfxkof.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gqzrkrnz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3igemtxcp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3houuuzri.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmkmtpfj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xgdmdrmv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3aiwdrrnc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3viqhhusj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ettyaxxy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3otijtgxi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mxysclnt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3szpcgace.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3urkpcogn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mhezlvae.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vwzwllrk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jqobjriw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lnixjhun.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3nixreduo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xemyapxy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ugmfbfre.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jnkmlxpl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3eyudgrij.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ezdycqhm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dahrxqdo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hotcflbl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qntitkjk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rcniimce.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qpzferau.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zituaqki.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pzvdweqz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pajndfad.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhqcdgxw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vvgavlfr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qcectxzd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3prnjrran.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lmgijnmo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wjzmnvmt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nmisnsvg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pokcyrrj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3danewygi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ycwlyibf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mxzkqegz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xpkszhxy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3durboipp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qibelijh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvhyrxus.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3eutskvzq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qogtlfua.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fibjktzo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xuqaomdp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mncthgak.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3auiumwxp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cwkgdstq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tdkjjeue.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ltvlbsca.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qlzpqjjw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kshyagas.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xswgognj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hlbdmkzt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ypjmzaiq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vavatxjf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3isxjblqn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xscmvoie.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntznypox.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kibotagb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wvlmzavf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sdrvwcjm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vjjbkcwj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pojgqzri.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jthibedc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ksrxijdb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3geceznjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3toawmjnm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3askspbyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hawpoyno.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qbonoqos.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wceimblg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hwymcqhe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jbonkicp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pfqjdhyo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ayjutrla.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ztvoyzrf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3asoevgsv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jqapctus.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3guyhihlr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bqqvgobm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kxrralux.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bdfflltm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ifgplvty.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yxrmxzib.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vtoqvhpt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3teigrtpk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vzouduzw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fqkpnjhf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xquusomk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3derwegva.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3oollwpez.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wbjvpzqh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3upzvnrky.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jnymvaru.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqopxte.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xvhsgjsp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3myeydljg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3daqxgbnd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gownnrio.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfirvbjw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lhhntwaz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3oltdebvb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qisawrnm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gucdoulp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mxtkrnya.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nlhwequf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mgcxczwh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yyvbinif.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gkehgwxx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qcuugvol.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cinarcei.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3aqnckcio.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3tvshyman.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qaxhvsiy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zjzxtmta.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vdyfdxpv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rjizxpbx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3cjrtfljt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mhjbsjbk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ovjckbda.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3oeolxzrn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mtlwobgq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xkzecpqv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tshrkikm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wxccdowr.html


<!-- 参考信息 -->