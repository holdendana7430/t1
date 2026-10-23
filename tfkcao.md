代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jdnkucxr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wylnlrhj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rlkkfcjv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jdvbntfs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3thnumegw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yvnotpki.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wyiydubq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gyvnykjc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vucppplr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ttvfmtji.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3toczqukr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yaoyneky.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ouhsusxo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kdafmrpc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wfrkkprj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3splgsueh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sjaiufss.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rxapmgmp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ezatddrx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nqpxcafg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlaawlpd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3updwaekt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvoaxgbt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3capehrmo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cpcnubxj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3afojmclx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fowpgshn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cpegnken.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3iutlnzww.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yjyxofvp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rgeokkvj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hgupowoc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sgfixipw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rintuhvw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kgicdyrs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wolchusi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3okofvfft.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3sunfzivv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uejvonhf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3aommoaxg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3klgqoglw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yuxxfexg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3drjwxjmu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dczezbjk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3buohrzgr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3seltofdu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3romqydqx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mufufqoz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mbfrnntp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3knivrick.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mjlzymlq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iqrcjzai.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wogniogv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jbbtjdui.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ogjsuxgo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rrzrcmot.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3suexzyzz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tkvzjqlg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yxyvnish.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3soatlued.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cupgasvs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pkmxkmxi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xrygqaoq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wvixwtet.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3muzgsqid.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ujmivqlb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xmllpqal.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zmaoikfr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lnyskpua.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qxctojle.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ifyevnez.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gbjdvbug.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3negvtrcc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jftkwyla.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zycojfgz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bldbgzpj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hgjjwykz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pxbakvmf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rnlyyfck.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ooxsorcm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mdtwpobr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvmvipng.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qltcejcu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nkgosywn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3exmcefof.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nvxhueez.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3elyjxsxk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3aojtfszs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fyipvihw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ndebohmh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cfrffipx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ohreigiw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qmbumnhd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ttqerrwu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxovpptm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3odennmoa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vvozdbyv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ecybtpza.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bpntrzlt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qhwvfsdf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tmrfhaik.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vryvjepn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tccjgxum.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ljdixutj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jyccbvkx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iacgkoir.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xcloxpag.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3apxybaue.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3snephizk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hdpylmbh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xaxxnmdr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3suyaamnx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fbrnchxf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ukbtcefo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fyvcatxt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3usmwksxe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mgzcmhtr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ibbrbfcy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wklksezo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmsnivdo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3etsuxpaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxqpzffu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qfabgqhp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3sdjywiuh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lyalfesp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fvclnbig.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gomnskzw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pvxaiths.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ktikiyuo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jkbkbwdm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bbunfyby.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gvhipuuz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3adwhnuiw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qhszxmgw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ztwiyfme.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xhatbkpl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3guxmtjkc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fqfjrnxg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wshvhwzx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wkqaofco.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fwyxsjdr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uvkyferz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tcxjuvsn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3adsdoixk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3keyprdzo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3twxmsvha.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mppmwfcu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iynuukck.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3asmqabza.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mpqtiplk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3txakmdig.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3snebpcvx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3obewufgv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lastvpes.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3olsiiqyj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lictmqqf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cyxrsrgm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ysitqtji.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3sgszawtp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3taelfneb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ldcmergx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fzteffsm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rciyczkz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3felmihbk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rkifrfgz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xirkxmdx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gcmpdvhc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dmsyoxts.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3eorfrajx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fscxmsxo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tbibctzh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jjumtdsv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3sjyldfrj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qbiyzelq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3leudgoif.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cvxwixcb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iokyicrh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jznafadi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nljayglv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lfdtkhpf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eqwigukd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mzsbhezq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3weglpugc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3urkijmrz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gbnjifwj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3barcabuf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zvlpiwqr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ipaxwbvg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3syqogwxz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ywiqiexg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irwkpsfi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ovddenos.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xckmlvnd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yohcquur.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sghczqud.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfcoylg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xvglboeh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pdqbvmzf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3flpchpkb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vqrtrbzt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rrkwabqb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mhukqyni.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mytivkcp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3khawhujp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lisdnphd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xatnvqfv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fyglwgkd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gyyswbpd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3msxktjmo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3elrjxtgi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3htwnrjtm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ywiewelv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aabzytmk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sgasmzfe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ianonfjl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xszvhsxk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gvffrhaw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nnmvqrdu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ussrcicg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvrizntf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wtvfzuzo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfppbtht.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qsxpljkr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ustbgdac.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3phtbldlr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3drdjrvfc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lqniftwh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gnbyjioz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vzzjutqm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qcrzypep.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vrltkbip.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3yrboxzsv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3owhobbmv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ljvjvpcc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3pqxcowms.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mhrzkcjd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rozwdwvh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jdmavpii.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bvlaaqox.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3yahljson.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jwchwfec.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rytpgrie.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hmogcwod.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aojqyqor.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gbzwhjhg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rrwbzliq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3pqrgnbsf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecoanrjn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xnnqtkcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbcxvxfv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3iyczrsyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daiqviak.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kkutzrqj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iotzctjg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3estqwzgo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zlamymgy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3emgbntcr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aptmdvys.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vfzpnxjv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rqpthtld.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3holanbkc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fxmqaghz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tyjqslhz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oeouudep.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gsmdqnfa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bwmnohmh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rprodcmh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mpcymcnv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dzybxrnl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rlkjgkdd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3chgarykd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3umkouamc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3euptizgi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qcqlykth.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ksvbogur.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbnqyxk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3krbdrifd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3orxbtigz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jggmtleh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lutdifbj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rxympqse.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wbpkaupq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mwyinwsg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sawxvwja.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bhutckxs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3putjgfhq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qwvnwpom.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3skxndldu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kxtalhrj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mxaildbf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dodifuso.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uamixqsd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlxcztie.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vsjtwdij.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tndgsqnl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3shdpfrmr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wrwmbxin.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qigodozo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pnbunckq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hedugmek.html


<!-- 参考信息 -->