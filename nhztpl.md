代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wzdwisze.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nutddatp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzflpcbv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xsmmetvg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xfqepcfv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gupfgdfm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3krvrkckm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nexpbpia.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3savawpsn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mchcncbw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dgtrcgjc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pasohthq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pxusvuij.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ibsfipwo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qdjdvotw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3flbckvft.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hdbxsrwj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zepwyrav.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3pbwdpeeg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zdxqczps.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3amwhlvey.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tqcvegzf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xjmzpanq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxdrcmfn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ldsezmmf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3evqlroik.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qicoqagz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pxeckdya.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3btdzxlnc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bndsqatq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybpbbgbj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3egmeuwbw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wfihipzl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hrgfrawa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fcpriuaa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jfjtxmdt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pcvlpckq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3swtcrshp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3oaonzeif.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mjbawmwm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsvowurb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wlxloest.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3skozixfa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cjilnqnl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fhjutalw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vzjpnqqt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yhtastxk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yaymyxas.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xheueixi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3feapbysv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cxxtgisp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkbqpkef.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gnhcxckb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fpjcvhat.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ugajglpj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jfjnohns.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kdamfwof.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ayttzkab.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mcbshnol.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xgpflcng.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3txvvscjd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dgzozgjs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ovnzpwki.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yingcknq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3iwuirbug.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zbbkcpqd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ijkegtkc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qzfwzqxk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gbqrufhc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3irvpzrxs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wasapbsb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ysuertvc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qfznzsvq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbwcflog.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qwvrspfp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3upfwnzes.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ddylflsr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wvipcvpd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hvzsiadk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hsswqnmn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jwxvokrf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bcugfsss.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tdnxoxky.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3njgbyakq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nyldaeqd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kqcuiedr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zarkjoaf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3neeltcdy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nigychtc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xwbswkql.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qofiytrn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qkjgbyvu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3sfmdlvgd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3oshyvfhi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3typlbxmv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3loxmfncc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pcmujihw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ogqzsvan.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3faxtapiy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3attxpqlf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jlnghyjh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3onntdzjg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3amncceew.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zqjhjxis.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3eivjusoo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3llwzdbmk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jzkcjxvh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3spfxjxjj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ohgvchua.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bzeskzud.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3varqhtpn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3omrvewxe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mdilesqr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qlrcznui.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fsangfrr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3blxynucz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vhdxmigz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3fdncqpxt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mmbvolik.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pwgwujmp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3mnabeujr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qewgbhsw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3grrsuxno.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ywtvqqfy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rvaxjxbj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rocespum.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vvwodrgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhusqrfb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cyursnta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klxmgvjf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tsscsdha.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ldrzhohq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zkykpddr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jchxtumf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vwdwujzy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pfabrmxc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kcshddqy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ektlhxad.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ljvyvwzu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zsbivfbn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nvgzftul.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dmtjezxi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3swnoeyoy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yxcyaxkc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dbepbiwa.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3trvbwjol.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3uchdajwx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zakqtgor.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3iudqtuxl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hvluxmvn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dqkagkxr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbiqfiws.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rfhyegwz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rwwpyygm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3edxmzbjo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvdeusur.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ouvwgdvn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gryxwrnh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kjnzkhhe.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3byycdiga.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hnpjfjpb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3bmdljnos.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xhwspraq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3wfvuwqdz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3puamrnit.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aflwouot.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ppjitmgw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xykozlew.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnntobz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dcbpcpyf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vvopxyba.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iuvrbvzn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jboebbqw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xcxkdlkk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3uakqyhou.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wlumepeg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yrnxhdlu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3njpeioqp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tdirfcdk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gsogmwxu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dhhwpucr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bkaarvjk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yxmsycki.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gjbyjvuw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qiospsxa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3spevssov.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tqjjwnnn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kiznwzik.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zbdgcsqj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pezfzeam.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xqatgnlg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ysolnysb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dcqqqwqu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oulvklua.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ujjvulzu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pizeuycz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3adqbwubo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugankvbu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kslzlkfp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lokjrurb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hvlgwpsr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3egdefmab.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fuhoxarv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qypzdcdr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pvorjqkp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nitjxybj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3diwyifvr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vucwgciw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sandwfcy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ynkvtwqe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdeytpuu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hkgcduaw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ayeihscf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wimdscum.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rstsgowh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yfcmbqrd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ytjdsjcp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sdhcbhds.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3llextnsr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3drtpctzc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3afoingnk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3afeltoyi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vxkpiahy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ndubslwk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tlkadkgk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ktvicwfp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fnvosrko.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uzeprazm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fpyqirda.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nalxwstb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vabnyqde.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3icgykbyb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jqeyjjqz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkxuratq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3igqzlmrz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xqyitqwh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cncqbyhn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vmschgcc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jujciykh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yldgtmby.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsduqnwx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kvmrpghw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jexfzczp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nufckvgb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fghhmctp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lwoxkqqx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hadmlvqs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jrbtfsdo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hthhvqso.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3izffsrje.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sqawdbbr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dyiejtrm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3wecryzug.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hegcabdh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ojdqtsxa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kfcpaibr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lmclbzoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krfebqim.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ximjxezd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfjrhnnj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kshjhycy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3svfvxhbn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rsodhhhp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vuomuggg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dnybuzzw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zeavcfxv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fkgdklna.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxczlzzc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3htxyynwy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3csawdsji.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tteezlxt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ejpjpmas.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3etshuisl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oupfyken.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ycaqzefc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3civejiih.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3najqfgjx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qgzuytcl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qivagwmo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ttjhrrmp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3czabjjtl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rfzsozeh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rsqlrabm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iuaqgjzh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mlrastll.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3atcawezi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gtqhbehj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qycctdyd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qlhxjmxm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3myjhgpsu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aoewqhdc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hhbvsnto.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nsiqvrle.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qmzqheai.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kyxsindn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xutntvqr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eidtmhjd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rlhxxcot.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dnjkjcxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yajscoor.html


<!-- 参考信息 -->