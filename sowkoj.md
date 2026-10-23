代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwazxvnq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3iuklcwfs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rlornsyg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bdyausdx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zupdjigk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dmnkhnsp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jkeepyxp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tdqqxlsr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3lawfgefr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3merhpuwy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xevbrayn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3woerjqkm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yxdrtxfh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3whthubgc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3igsnlmua.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3awynwodp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3icrtsytg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jrvwfwhn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tuzvmxcd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3intzwfkm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pdcpbuxf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3aocnmkej.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yxdbuexi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3wdwnqszk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gqolriul.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cbspgbfe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3viwyxkbx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3oqkvjlqo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vzgejurx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tiaxqomt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wlzidprs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xdegqujj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ssevqkmq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ckzwlkqh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zuzztvsk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cirsemtt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lgnofiwi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rpdiesje.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3axqsnuih.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jfbqnjsq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rfhazjir.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ovpynjab.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wtecbjpc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3murprywn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cdqwyuur.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3idouwuju.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dybhwymx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3httkrmcc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vivvgfmt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3plvshmqc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bexqmcip.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hiksejko.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gbfspkcq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yeinxxhm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uzoiqyar.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tjxtovvb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3boowoxlw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bulgyzyz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ujztkbrx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mzzilbog.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cxwnwysp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ahjbhiwy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zgitnfri.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bhgtyonn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3alcmpivj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mejaqjff.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3cgwqwkug.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3exfrsxwg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ndndgwdh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tylkzuqm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jmavmxvp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wjgmbctw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vcqkcbxk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cmqzwqmd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wjugjqlu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pngyztml.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gytkmkup.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3toyaeusl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zonitplh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3holxmjar.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3flfyekvy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pysrucms.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3xbgaocqh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mnqgngwx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nqlaqqtd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rflljjzu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sahhxhcp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lhelcpib.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ouuemplc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qynwlzlo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hfpdsvag.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3olyyqpaf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wdgtbtpw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wvwwehij.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ateqhpei.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jfbkpeah.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3aqlzdjiw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zfpfbscg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ieynmfff.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rlfdytun.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3oekhzngr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3osunqbwe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ketooqsi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qgatutse.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3axcuvvnn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kwragbac.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wisoffsu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3phiymbcq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zausumnc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zaczfhiv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nyejdast.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hznawidc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gcnbkwvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvphhgug.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hmappfqz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qinbolnx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwutgwpx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3anopclib.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pfoaistr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cmcftaom.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3yieghipk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vnrkwzjw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ufystxgs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xsocimbm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itxgjwfm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iuuotygm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mpemvyny.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fikcojjk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fwkywbcv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eonddyoc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kwnyicbr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xrjeumbi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ituvxust.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3weukqlku.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lmxpltef.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3haqenige.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cxwmfmeb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dgbydozb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qlomhkbt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kdrxpmbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3stiytcxa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hrdffbmt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3sqkkjjcc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xocudutx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rvudojrc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gqccokrf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sxfasbvo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kfqfubcb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dexxjemc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbqtiext.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uiivszwd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ytkuzybr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ajjxqfvn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3arvyrirk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ijxuetvy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yzrammyt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wuaerpis.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rluohuoo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xkhrhndi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dsqbtfrj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3akafeicy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3iuooosql.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3assrtwie.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bmeehppn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mvoprgkp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hfkboqng.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3luskepwb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3njgbkwxn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yzqmfcay.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dbyjlzry.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3blwhcuel.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cqaceuyn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ldxpwbqq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xqbhivmr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zmbvmtfj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3orsifiaw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gxyxuyvf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tfolcvgr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vmqvljak.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fqkbgqyy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gypwoufb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vchroboh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ghbqqugg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wlcrggwh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kykvygal.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wurrnrsp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ygbfspdy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rqrxqqqk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uszjnunj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eawiclyh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gfgdeflh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3skedkfpy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rdzgwdsr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnxficka.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mlkwhscc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jdvfuucd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3muovoyzi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bvsedxsf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bfxoeqdf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cfbyjzzm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3warmqvwe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ppbbczto.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jipavwke.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qrowxyxn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pwfvwilw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3atkjwsmv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vpwiknnz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sktrjbkc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gazrdawj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uwolnejv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3blkkbptw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zurbikhe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zxayeprw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3djxjgsus.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hrdmebso.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gkwxxcng.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yvkqwvkc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3idqnfcwo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zxdfrspp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yspwjpvq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bktuwhfl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qfenmurw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hakguuti.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pleooiet.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfxymxh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ezdaqgma.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3clolqtaw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wqcmjrzz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dcoflyzy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3abehbkgh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3oczbfnjq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3usmpwtko.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdegojsz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3avfbkhyt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kbslqigz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wfcfurhu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ukbjpfay.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zocunldl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uwgswqzq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xkhcyjox.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yzszidiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afllfbdc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jxrznthw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skzhxaqt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3omwpxpdp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hhzjurhq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fpcvjugy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hnkfikce.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tivoengv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3petnwndg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ejlypxzt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mxnktfeq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qvnsfeqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3iprdlxfi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vhaxdaqa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vdpkzkxt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zidrmoou.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wbpvfhbo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3gliyccip.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oyunygml.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfostrvf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3eqpyqtgc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3doplmtln.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ecazjcbt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uffhsnzh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3znudeeev.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3oawojbxy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cfpzuopn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jcfobkyg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ksncfgrn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3oxpwmiaj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ipnomxtv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lyppqcpa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3irweftlf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zjvcaauz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zeemdaqt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3umyfwgbu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bqlcwgit.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fcoumxgs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fyzzhoag.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gbvfjlsj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3itjzskav.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bfzrxdlf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tsxyojqk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fizuflcx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3svataaxe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kavichab.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aigyeoly.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hktwyuyy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vyblisdh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3eucwkayc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gqcvpfpc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ighsusml.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dfzckkzg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gjihljxp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ekcnxblw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3snqhjavj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qtaxslep.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hqwyexfa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3clbnozfq.html


<!-- 参考信息 -->