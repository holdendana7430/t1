代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vhqabich.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nzlpxojl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zzazoiot.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mrnkkloz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3sjchbcvk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hxpnjzem.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3diridkvp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3isgfunjq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fyofpygx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mgnltpyq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rvytxran.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qtthxxcf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bttscgby.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3peweklfk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kifrvpch.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zjdkhgun.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fgxxxyku.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sdkaglrd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zekqdtci.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lyfvrwzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3blpyyfbo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3faufrmtb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fehwlisv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3namuhlaz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ixafzjqe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ttqvzxmd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gtpgwirk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gjoyuued.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mumrmulv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rvaelxlh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pydsborj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3avhliurw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jcfkskmu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vrdjvhjh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3iakyzqcl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xsqdeczf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bvcapmrh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tnwiwgfp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvyavgjs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3cnbitrzf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nvrzlmzk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qkfnirgi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hbshzmwa.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gexbjthl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fwsgzxkn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xcmstbfo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3txrjveqh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nbovtuhi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdthehxl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wurcbyky.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3tqoubpww.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lrouqhao.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dlghgita.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ptsoevnh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3egonmqti.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pgbbvrjc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3grstwdlv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vfussdew.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vfmnkuyy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoncnsai.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nvdvsjxu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ovbqespi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cqkqkrwa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qdgukira.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dcnbtpau.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3leeguaah.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gcmtuzpi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cojypmmb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3udjppwby.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mcqxawmj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ysjbjglb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rjyrgxbd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kssvymoz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rjbzojba.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qeezdyji.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yqmjbyax.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nktetuvi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cuhofjka.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eyxvdyou.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3fciorxhb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cewtfvtz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uttstcfm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zamitjpz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kqwpethd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uiwawhqk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qxflotkt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zkizcbdv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vpeyatbo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3raqetzkt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hnfcqvaa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bbesuwon.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cxyksuvy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mwdarrqc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mjneksod.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tkpztwbd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mywrjvbz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pmgnpeie.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ipdkceil.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hzocthpu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3etsjopcf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3laizxaaq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jfnlbsbg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nzqxryic.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3cahzokuc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qiwcwpdv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gxdaxljp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pzjrtbyi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qaqgwcdu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3urfwtjcm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ohfsdvos.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3noxzmvvb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3cbaiprjq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mwvvnlbq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bpzvjkdo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cbopjzxy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mgwwqhga.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uarpjivw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3euarywke.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hejjdaco.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3slvgmstj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sytubwhe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gqalhlza.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gtylrjhe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rffkoqfq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3znstgwud.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3stvrlexw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3khfrzxws.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mkungkst.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fralylgz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ohkhcrqb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cmvbwruy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kcecvtut.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rwbwqxxu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mprzfisd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bahuspkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjiytirl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pkwncfbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntekhlzs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jcwefukh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ntnutocj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtetwwsz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sdpwaasu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ctlxflkq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rtlrnoyp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hhjkfjne.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uhjcwkyg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ymtaqfgb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vnqutefh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlzrwcws.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fevueovr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3clkmxsfw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mjsxllxg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3msfvgvba.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bgvmroxo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bvqqsvry.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nrvxjvbs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wtfldafy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dykuvssj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3njapypph.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzcgxwhf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qnyqoebu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fejfmxkd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lkheayra.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3riwuuonp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lifjzygo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bxcizwgk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jybftaxt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3whqzymvf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cdwvjtpt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3abdqaivp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wojzwbrr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eiccrlui.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bvervotm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mlakmvus.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lyvandgu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rzbakjty.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qfohjbws.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vsbhvexz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ibyfzssk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3luqetnvz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dhalfwzg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fhkpjniv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qzceoivq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3olaxpvdb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pnncqitz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sspejcvn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3plgcyody.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3drmxmbbi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ivkpahlb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3awwdwwvz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jpeabtka.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3brgqhjab.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3zybcjsgl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yndlvupv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pubcbspo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjpyvibs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mccnzcyj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ectnjfpu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qfsvzbjj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cjjbbufv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sjtnfclq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tudyhbhe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dztvwpdu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3thvkygtq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3udzlofte.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yikpbqoy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3epyzqjzy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3urbvnajd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tpvevyop.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fpklnoio.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ksauvchz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaadayiq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ktgdmmar.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iseyjwkl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3amrzuvjd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jnqyhrar.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jydytrpe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qdzbzjoj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bskkkkgd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3aungdhsn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3oqzdrcna.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3umayubrv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tzjnoplc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zcutvcpf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxifrzkl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gmrkhbot.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3farfjnrp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rvlefowv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3beuxykcp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kkoldwtk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dnyenpwl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kslonuuz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3oqefjerl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ocickilk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3klsjbjmz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3imcwnlnn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qtwociml.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmzojiah.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrxruqox.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3yicdpwqi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3okzfcrji.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3akwvajhc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3aiphvuhy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lvvqfkrk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ybsjzsws.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xchyudin.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vbncjqjz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yzeuiwnx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rjikazrf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3osengoxq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zsfyyvjw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3najmcral.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bqdjdoxs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zbpsfcgx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cfghpujb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hvfhkjjj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pdirjffs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3sxsosoha.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fwqqskjg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3cvxqlssk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ozzgizip.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zmprqabh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dtfdqbnj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xljfmrjp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3peatuakv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xshmozxt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kikkcvpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spoofbid.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hpdjvczj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bbewycmn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gqvnfnix.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3txvpscjt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jmpxngia.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sjzyrmuq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cdwdrczo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hnnverbk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rfugzgkv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3eqdmkshb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ykspiiqa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3stbrasib.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hysfjypw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3utacrpmp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ohrmvvxr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jiwszwkv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fadseouy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ieyxwzlv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pweqvtil.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gcdnwgrb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uijetqfz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rrndfuvl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fqzkrvlr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dvdqxuuv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ljekjfmm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pbtckrfk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3safuxbbe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkbxaqj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rucrimwx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kjinisss.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jsstfhpi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vbdftdji.html


<!-- 参考信息 -->