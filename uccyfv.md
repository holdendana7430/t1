代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3iqxfgigi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3grkutyqx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dsikebxu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3chycrzna.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3lnspynyu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vritlnkj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bynvxsnh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rmmjwhpl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ncpukopq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gtjqgkzp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xibvospr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qnfzuhbp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3piojfzeg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zlqjqtya.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3toekaiui.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bovbvtrs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vjfblnpb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xahctpxi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iqdreuah.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3laszhtau.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3duqtbrdt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3uthmhfqq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mchqcdsf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yoqkdihz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3disgnvsx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nvpteqms.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zedffbyg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gcdqkivt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bnqhsjbp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wdudlmej.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ghwhycri.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pjwyetrq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ovvxxkrz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wbwebhsc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mftlfpil.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ypvkjwqq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ykntnplk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3lthvhewl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3iwnvlyeb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rmztzkbw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3atxvoigu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3whmugowc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ntxuksho.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3iyinmiyl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bddnlkqn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3murciztn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ispbyidv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xgeunfct.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nxtibeoq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wnpvrkzp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wlthtyob.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jzhkzksd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pokfwzuk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gwdwyawn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nosfalcc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wfsjzrgg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3kqrnrzmj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kuhqmscj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wsucxttg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3uaqvytqj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wvsbxdhv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jbaftbqx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3eazgizmp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ioisrjqh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nitmpbbe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3taeekamk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fshmowzy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bnqruomp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ikmtwres.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3plscoxlb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3piugtgei.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wohytain.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3frucxyik.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ehngrvss.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hevayxng.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ecjqebrk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nuwxgges.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wojltvrn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3augaicur.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xomooojg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3icpltbcx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jgdygbct.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tlfcxsin.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3naqckozg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3azxzyrja.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3olrjdfeb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lojpivnt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vbikbkuz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dtvoqtbs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvnnsgls.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iajxflke.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bszvilwc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yirdqtre.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hqvgsgeu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dzfehwfr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qrlcyjji.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nmdwfpnr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlzcasnd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qcdqfalj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fehiredp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3erhmnaeu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ycxvkapi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dlcoilyo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lxgnhrak.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pkiwckjr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nlbhplpm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ncuaifqj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dzzerygq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ojqsgwcd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rvaqlonh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3skxcsypf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kllczmyl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fbxnujci.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gfgewnra.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3srsdhnqh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3sfumqvhk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qcybtsyh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sfnknpxe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fwqlobbk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3giutljmu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mhgamrmu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mgurtjdn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dijhhozm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cublmxtm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3berjqdwd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nemxuibj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3urdlzdqi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mslhtyfr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ksknghar.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lsnnflpe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtguirhx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fufpwwdw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mmfhjput.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpuirruh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3baudgzwg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fazsdqdn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jvkdvmgc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3abysoshd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zazopeln.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rinmrptj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3rajdkmln.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gzbndtgk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yxtttszv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvexhjae.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3exelsnay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwxdmdli.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zmwnljxm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fybfqduv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3trwyextb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hftfjutz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3azsnshjx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wwyigxbn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jwudapdw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kyiowmka.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fwjbfppi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3whidnowz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ocjwosbh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lyqictes.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ezwuvulg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kmpuxdue.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3wkkqfgmp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rkwyhqic.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fmkhaneo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cqlbblvz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3etyfjkyf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3swuwvosg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yjrkuvnk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3foqgfmha.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lesmxrsy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wuiocjmo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ojicyrjv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ivwnfdzd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lhhkjrlr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qlguaxbc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zbisjjpv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gptykpsy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3icnihqgo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3usljztfr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vutlnsjf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zzdhypai.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vrdtytgn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ebjpeikr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cauwswzj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kpqjhhgv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dhyqwssl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ybpgjouj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mivirreo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gommgszm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ptptrcse.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wrdniuhl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aitegxfx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qnxzkmbc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dodjrnqq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cvxvetaz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ejbklvhc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ebwtcgpd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ypzhpuhq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xjdybvqo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ibfyqpnx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rujbonib.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bsmacrvn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cwnausgg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rnglpnru.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cviwytov.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ovqktsij.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3azrwipzj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ejdlcuqk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jdrmxibo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qwoggtcl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yeuzzsbz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tdmfcufi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vjstkraj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nsasxiui.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zbkfatlw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gbxuhqhj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3leushltj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wqfjlwba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjsnggcs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hvsqzpuq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jthpcunq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3unyubckj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qoepanmo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3igujznir.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3elbzqvwm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aqxbhhju.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ucowrzix.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ayvqcdjr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3crwgsymq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3oqfhwnut.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zmpqpspn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zfdxgsoo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kofdtpcs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydmiexpj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ocicaonw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwdiucrl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ueaygkqq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3prpubiai.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ooynfpzq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ycxxbqmf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3soecrvex.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xgkjkyem.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bqlriqhy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qvmtlesr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ywzwbbmv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qgjswkev.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ithfwpsg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrknyfua.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3isooktbq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lgvuufye.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qrooumcs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3czpebmav.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3svztxspw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ywjqjxjq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zqvucygv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wbtnjqjr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gazwhfpz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxtbezlj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lxyeujok.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mmxczlnu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wifyitgw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zdvcbboy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3pmcjyhpr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yixmzllu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3andtjgax.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hnaxkoji.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hmkttelc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zglxpbfp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sqmklrwx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjijiau.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3guumtgaq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mzhkizca.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uhivwhjo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3czrbgpwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gozoiiec.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ncsycnle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zeeuiygu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yktjfncv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3waaywodg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bdovpbun.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zremjuew.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qnoktcyb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ftclbjee.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nfmmkduw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wsqqkgvb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cwafzqrw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rvcsinrg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wgiwirsk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fgcbadsa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bbpbymsi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kjoipbqv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rlvijxlj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kyvywlte.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fehiqddk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nztfdkqr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tuuclujv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3nieolmvc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mrnehgvt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ldtpwnjl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rtvyopcj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ebbgcxho.html


<!-- 参考信息 -->