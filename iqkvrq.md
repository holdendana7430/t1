代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2etantylq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mgvbkreu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2enhdglsp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2phfnwaop.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kpxdishn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulwknbey.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cnqwwuqx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jfqkjgno.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tmvotrjx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xgvukcsx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fxkgupma.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gwrptipk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxjfzspk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zqljkwog.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oqvdqsge.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2aicidzit.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2npknjxwp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dntxsmlu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2flzxfned.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bimboyuj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fjsfnefs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nzklhjbo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2epndhyby.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lsnsygjz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rjzgocty.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dhjnztnp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkqgibwv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vcqnyphz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gsggdujk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2thracynr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jnhmzliq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fpudiadx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hbxsunms.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fpcpizib.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jactwwwh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pfkiguwc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kjgjlgrb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yqsbdous.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2eldxlfpv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cnndfltd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pkzefqwq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tvhfrhfu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2plybmrzy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uvgszoam.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2iatlgqok.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zelyqcpy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vvgmzjrl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zaxvrhih.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vwgsaszx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2byolradg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2amvmumnu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vgjejftd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kegqmgux.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2odgjwqgi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2oatevvba.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bsovmhpg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xopnpyzh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2oustszqc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pauaniso.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wkzctsac.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kwrnible.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lwyuuzxi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2cyfeadst.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tyydfubb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ccmhpzad.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jzvmyksp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ozykpzgo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xxspudvg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nctiizxi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rcqnqmlo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dfcskqtn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tmvvmykr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gnwdmter.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2himvjdsh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fvfrtagr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2igssypkp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jlruyhze.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mwwdwnav.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mohemnvq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2oaobxoik.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2njbfzkpu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zjfvbqgv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rfkslbrv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jtzcuthd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rwvkmvix.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vnofzpvn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzqdfwog.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2oqervoap.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tumivppl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zaeirxtd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bjzoukco.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tnsldizr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mzdlqyaj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sgfxoxij.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hlxbmhlk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fbpgmzki.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bhicosso.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ocfdqbwc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kpqpqhya.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qbtcoezm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hpivynnp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2neuuwcvj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mlvrronh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fwnbmkot.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ydcqezhk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ahlvssyc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kykntngi.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2derxfmnw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2moobfoha.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ftwejxhc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cwlalxdx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xgivurrx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2eulhsmjl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xbvxtipg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2unzdfwvh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cvdlsasy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zyxsrqsp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rtxbbwby.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wcwzuqiy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2erebrbmz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bempqsji.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wypdguty.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rmnpspas.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gnzdtzue.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uzdwyiae.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ppxauxoe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ycjstkkg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2afidvysr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ppvyzlsl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2yhnymway.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbvuymea.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jyivsrbe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ojhtiztl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lncpgokf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2spjdwppx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pjueentf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2iponwvmi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ufzfnwip.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2sotfkosm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kgmwonbg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qugkczex.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vqammzoj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bwywwkuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbmzmbwq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2boqgmmkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysjjboko.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2spemjqjy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cxewwctm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbllmufs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mzfigryh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vimuxfnn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2uqyzltai.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2htkkyhji.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yhhqvzmc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rxxrpvhe.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qlqkmotu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auxbnlfe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kmwiobfy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bnkkzcko.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cmyenmyg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2orqgarhc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yzxcymku.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lkkwguyo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rgkrgkql.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pwgfwqnm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nfnoqesl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dtunoiyn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2muiwyrhe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nbihdvow.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xyrmedld.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2refcjhrp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2augqtttc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sycdwozp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2etdoaoqs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fydfxyhv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fzpydcby.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vlyvaojm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cnversbr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wydekdlk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lxyautqd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxhqvohc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tidnbgov.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wxphzwmo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qfcegsqt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrfjyve.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ncnzofxn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oirzmoew.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2onyssdpz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kaeaquia.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hfvexquy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2veurkfqy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2irhjkjuj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gurqwjyp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nbuxjgtp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dyeqshnm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tlvauarg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2abvnnaxs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yoyqnred.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yqulwoor.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2loobwkca.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zzupdpkw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2npsxhwit.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2naaegrpp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tmolnxsm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2aiqcrfkp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2eeuheswa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2sksclnys.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dscgybgm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wuxpcwkx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vhqhffki.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ccvxqudb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hyzbucmp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2houwhwdr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2miabaivb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmrtvqms.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kyymyjvv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rgklmxvr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tfyyvfmm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dnqeyhho.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfkcdngk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ixaqbuia.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yaxaeixu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dughhlin.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qnrnxjvt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2orrceejx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mnhbfovm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ueypxqli.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ilvowcup.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2aebvnchr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2omkkmksu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gztcynhd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mzlvamdo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2djcimppo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fsgxmzex.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jlmvcygg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kgpjabsi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uppwzeru.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2trljtfpf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nkrqjnuc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2inosbxxk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cimusowj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tequdtql.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kiozxkpn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbwogttz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wnfbuvfv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rcexkscq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmalnxhi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jtpsjett.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zzfxxclj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifafrijb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yfdvkdtw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qnyikjco.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fijnluco.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2eypfsgki.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2whtjjfxu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2kxjlbkkz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uohfqeoa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pgucjwsc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qqzhryzf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lwutfviz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dxrqbtph.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tprtnnxd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qiumtzqp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dokgvidt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbafdtcg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2buioceov.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ntqvzwkf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hiftsiwo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2khayuljk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2whlbxaqk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ljwkngza.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ehernwzb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ailjgzld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwmjcozz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kgmgnohp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpkbgqlw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mgltnahi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2piqklyms.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwklpamu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cngdjchz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ruwrimyk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zifaqnig.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fyoblggp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkffgqzm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dsjyacrr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jpdgodru.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2smmbceve.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jtxaqpdu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qshoyaua.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vgovuvgn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2homzdhxk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ccbbrtsf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2slxtpero.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rwupzjqh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hosnzomc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hmkdpgup.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iqorjhsl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2axpvtnsp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pqxoqtef.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggpcmbhb.html


<!-- 参考信息 -->