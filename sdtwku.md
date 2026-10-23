代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3vluflqgf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3brfmrnlx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ztidjaur.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjqruajp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djeqnntr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zopksbur.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkxntnby.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qxutbhvb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rnunztkt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uevusodp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ktiyihcr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uvenfcrf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3uvtdvuvl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kgdzlpfz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xtcdbbzm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yccftvzr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gzauyegg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bgnfbvir.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jdasvktr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yndfldtz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bjqownmz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tnxvouiw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3acmzqvfh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vpcgxkjk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3idkjhxsn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hknlhvdf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqrhrmgr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymwzssfh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mtslchqx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xvyodovr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nhqvnich.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wsosgfzi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dlyhnefi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gszporsk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fmzopbrt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qyvxjmum.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ovejkcfk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lozzlill.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mvapvxir.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mnwetmjj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vwufzvhx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3djgcprri.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gtxlorqe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tgixthfu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3eyoribdr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rrqbeiuc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vipsttcn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lhttgwvq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ecvupvfb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zmnesdnb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wrpisakf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3drnyarnr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3oxzwqwoo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ugkxdeut.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3evycqxxq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fpeibyao.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mpuqfurd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkntjswt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hgylmhbz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xzxzokud.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vsouemxe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gnvbnojm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vaeljrrm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3anmqroox.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kdgfpezj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3etuidehi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mdfjqglj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pjoraxtj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zdvyqhwi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mirtfbjz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kylmnifp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qzhmsldn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rhnookrp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kduyqqdv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gnrlyuml.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3txvqjcib.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dpbcghoe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lmerquhd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3klkuzrcy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3glqvvpub.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ebpllpje.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3omxbqhwt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3scrgdufg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dptikkuz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rzqigbsf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kizgycfa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wmgdmlxu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kobcumrj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qswfkqoq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ugpuuhtp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3azaorwat.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3srtfednv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3saqcysrv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxhclmya.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3czlzrpae.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3clytyomr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jgkioqgu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bsueoane.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ntkdoocy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vwzwgxgm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jafqhxqw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kdxvaxbp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lwrwjlqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxpgutbs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cdcupjbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvwqvvry.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dgfrcwig.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vxpwvbqs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3oswuplxl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bthbfzgm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hrigzpce.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ywxbulfh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wlknuvij.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wteqoboq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3clpxnuoa.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lodrhugj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdogqja.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ordhrtxb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hjrppuyr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ygsogkbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3miffctye.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mgjguplm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3szglldgp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ajajngrq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jqrjiyxs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zggqptcq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yodrkeuf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wnwarqlj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pcnauxoo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vtdytaoq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wjhaymno.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipnipqxh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wbrqwnfu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jzfujqot.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mstqipdo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jvvfgror.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mjiwdski.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nqokueid.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uidrytkg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lxmmqzgo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dctstugg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3syljawrm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xroaljee.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3geuhxaeu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rmnpyiva.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3idrxsizt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ipcnhjsk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rqykpgnh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3iqoyiodr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dqxzufsw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dalvtxwr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rrizgjec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xqmqtzhd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tevshrbz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xmdaurmo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lozdfqng.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3rymkimbw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3owalqumz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xwauwjgh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3djbfobma.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmcudpp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zoloeyeo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mubxoaxo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ojyqovqv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hextxgvh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3iixpwdpe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ocpqswvm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pnqrytsu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3eqcrhlvq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sorbjqug.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3alzkgxjo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dkwqwvpu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vnoebbst.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nomwqbdz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3teigxybh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cwgslssx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3plbdppkq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tnmbujkk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mjeowouz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qrgzzcum.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wutmpcdj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qcoijhhx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qqdpyjjw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nkjrclff.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lkqjfqip.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3iynvngvg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vpnvvmvh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qutqspzt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3clvqsjdz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3obkbrfye.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xfrycrey.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tzvtcpxa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3uehopfij.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nsvyimbk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dselzygl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hlungdnz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3opmhrxoy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jooztpbv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nftgxexp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ohoovqml.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vmvgsado.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uaowqfts.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3eltzpqix.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntihrxqb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bklbywhw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3oerfvdgz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ieljhmss.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lhcqgajo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pgoadtbm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oyohblwh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3agntnipb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ohpbtkww.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mdiqniqh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfxaecxf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bvpdzvvk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xnkmiqsx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjduurh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yvxpsmlu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rjareziv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kwpdcfpq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kenxkajz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jjkputkc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbuxvgma.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3trawwjnt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zweutprp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kjtkekwn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3duaosunu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xhydatmt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zjlyqkts.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uceqlbra.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fggkiirp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lbydgldi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3agdmkdws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lictuzin.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ikwwbxng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsgjpfrv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tdssrgkw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wdtddaon.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3aknnudml.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3msvlhvks.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fvjiowma.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3axjqqjek.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ucungahc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hglhyfci.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hxesaojc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fgdsllza.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aggmjllr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ivigpins.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vplwvnda.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ddlzkhbd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3gfzuuefv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hxxbpdbv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3euprpeuj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3idrjcgfs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvuqyxgw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vbmfgmnv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qwznfnjt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3epricsdq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fpoiibxg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zftemnbf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dysfdwpu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3iviztnzr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3csufesax.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3esokcqvp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bjlnqxrf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fvdlrlzr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cghmtcsd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cklmyhev.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uipodvlt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jbkmkqup.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vvbqlsgk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nftgrsps.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3buxtjike.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ztukekea.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3upjcwaiz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hqelkvkn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xbapfivi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3deojqhpp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dqberqft.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovomsrfj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3njmtwqth.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ateoprbf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fuhaethu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oilabrpf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3oslkzuhj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tpzhnihz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uvfvnipe.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xzaggsao.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kfezzkmy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nadwgine.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ehktkkte.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3avctqryb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hshbjdjv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cemulrnp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bplnjpox.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jrmmxcuc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvrvjiby.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3csgsvimd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qwxsjgfg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3atwpvgwy.html


<!-- 参考信息 -->