代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wkfxnunr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kszzntmi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sqxbuxtd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nibzzzzk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jbezkmca.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hkrgmhab.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hkfupcxk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qafkzikv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iseckxpc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mqslggzt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pbginixp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xsvltqno.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dowyufss.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pptgqvog.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3onffddqu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3syvqisyy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bcvicrxp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3awzkegzp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ugfqxlei.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lxbpdxek.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lctybwsb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lwvlbtpv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3tylghoge.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tsgmufef.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3edxrljiu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bdyrdals.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kqzzxkbi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3elmeddjt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjrinarz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uoipaaco.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsrvsuwl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3iewgqjhp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bscpbsqu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zgoonlli.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gdapekcz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3avtwdghp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kftvyuxk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dzsbtnmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cdlyejkr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ldpggvqb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3csvetvfh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hkhoajbc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fxqmvmlh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cwpcnhdu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wcceoynr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3azikzlaz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xofkhfly.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nyoapeec.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oxgmolwd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ujhznejo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3bwcyvsqn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qgmnnkoj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zukcpotw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bltzfeki.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kzimkxjz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3afkschsu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vjyouthe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zyjzanqm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lgnpmsbv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kojgtuuy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3edpofhpp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hdrfwgjy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lyojvzig.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3peyvfhgw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3krnpdbxr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ymcjwbmw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sfyyotki.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3htajwjbo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lpydtfox.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yjtdpzeu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdkjhziu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xhsktalh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fsegzxwg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3htcitsso.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pqbrmpup.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fpslcmyn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zkdqtvek.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lvqtnekt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3syuwswsw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dvlbglys.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fysmejba.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ehuidptw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3exeqzrah.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xtqfxmqo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3czfcouxb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3huaomodr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mbjeixuw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3czalkqms.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ksroyyfi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xwrnwtpn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aacfaamu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mgjtukpu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vpyupvdm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gmtmnpbi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3uvcraflk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3coenindw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3udjxxinr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mozxvfii.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bjcmligg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xqctmtws.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ugnklekr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qkwuwtzx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3notuuaml.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zkeauetd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vmmrhcss.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nkailuwd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mmugrqjl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3omykqmqh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xzcgbimi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nodhibmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jfessnof.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3juxhxodz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3aclytqrz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pkvytyuh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mlilguub.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pfyjktqv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bdnjhfad.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vqnlqeks.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3moqotoqf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xbsonsnu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gbdyhlza.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pmtflzjc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nnlnwext.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3aknqdhal.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ldlnlrdv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3czzsxstf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xcqvqhuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eixybrdb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ovevrwfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujqneibn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wsbqexty.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bywxvhqa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tvhfnsvp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3epapkcgb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bmbtmcma.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3totunndk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ebrhqryk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cjkfloqz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3azhslsyq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dsebuhgh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abtwsyjn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fgkmippp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lkjpvuie.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ihwvprnr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wawxykup.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3luqraznk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tnnbcyzy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tkmczxpr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nkawduar.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wjsolsfw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pokmixlk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3geeoajjk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uksnqhlb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qnihfxhz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3njjdbsel.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tgvlikax.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bwpnlout.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3apzqnyrd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fvymkevr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qeiwxety.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rdzkkbsz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tmyaxdmw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fipblowp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ssghpevu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3bukxhtrz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qyffboco.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ofzwpzsd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ffrdzcnf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3cnmwhljb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3uelirnwl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xravtkwm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3chkfxfsw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yaxvgjmg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gqzjwluh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hxufuoxq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bfzfzybv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3iwyzprsb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xekhgcjx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uldskreh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cajzofll.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hdeoprpc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dvbgcqtq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iurfzxjd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jmadtadb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xdaldjcx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3magibcpj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3koykwxmx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ygynitre.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vpxphhyj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ynuhgdkz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cpncsxjh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nouxshwh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rifvrfpo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tluzkckr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mxjcxppd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lfljmjna.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ehhwcseu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nxalgslc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ityvcnfg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3izubozfq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xonvedki.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3slgfqbap.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3grqyvhai.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmoxqwb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3htbellyf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aeuvxcqi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3obejgbje.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gzpcvhnb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3objvtagh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pleandnw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3khgsvbgk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gotyqvxz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3veqojwjs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3skfeyoit.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qwcrsefw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vuualgva.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3taspfdxs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3gqnykeqb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sabafqqc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3iwvqjwqk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lkcvvndu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hqnzlyuv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3weqyaynv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gefoapkh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3odetyzwr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3oxgsenkz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3txcsumfn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3atkryfqt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xsgatiyf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uepwdsaf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uoptawon.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xsycglnr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3yywevpgx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqwyxgwh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uwddqadp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3veueafxu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3djxpxjjx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vhqieuaq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bdtwnqxk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jcdfihuc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbobxaq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yqkuhxyc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3npkxtvcc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uknvsuyi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ftcpligu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xfsnyfzr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jtnnvddp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3afetpfmu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uttufnnt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vflwhsoe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aoocybof.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3leytwuxw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ognnpvey.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fucngcnm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fxlhwlje.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pndiisvq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3erslsrbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrcinrig.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3myriyroc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpzbzufw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hjnwzqlw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3svcavqab.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vwonaewg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bsxsfjqw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kouklegu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kwzaelsc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yjjwtimc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xprmkxgu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jflhvplt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uaykmuxo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ycwtyetr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gfkpfgdw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rxxzekzc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysdexrqa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qmoyuusb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nsbqxsjc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nexsbfri.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3faqiwpbw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3mtdexadf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dezwzjdl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xusrgdnv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3slpvaiku.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ppxdrcvf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvdulsa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wxffkhsj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfduvwm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fmqbevnw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3thyrhegf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mwifdsjo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jlixwncg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ueybdrrn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3muaxafvw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lupcdacm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zeqnhtri.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dqtlhrch.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rmyshajr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cjprdsea.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vnlxqxco.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wmncpiwi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ebyhisdn.html


<!-- 参考信息 -->