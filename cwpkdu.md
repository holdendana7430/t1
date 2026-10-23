代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kmskawuh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxbzkgdu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qqcfkfkz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ydeshtzz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3twfusogx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yprvtxwt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3halnqhwb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hssuxups.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fvcqtpdt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dsdnikcp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ldgcongx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3emmpeqvi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lkmuhvkt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kjkyncnh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cyzsucmr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lqfkzkgc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vdfneiur.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3axrtocan.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3djkgewqq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tvotlcmd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3baatsvzd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yecetuwj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3btlnwaxe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ntbdflti.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ifnxtxbt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nrumedug.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hpaoyhzx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzzjokcd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xuyjhyah.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3htopvhrl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dlsrtvds.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fbootygn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dhrwfllv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zbexhkiu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oknbmcwu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tvyldjfg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hzhnfqfg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wkbhqkkd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mhnbjiec.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ltpllwky.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iptkateh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dozhdgpb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3scfllcyy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3prmrlqew.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3iqoxstkm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pgdsmkks.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nntquyvz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vogbbzqp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3eipuinuy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vwdaewnp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3anyorlbg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3pdnayqeo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fbohjspw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bdewwwmq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vuneiijw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3trllpqpl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ttnhaaxm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jolhwgte.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zhpkqsek.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kbiidlcn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mqygbmzc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bsdrtiau.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3omfyfdix.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bjhoisra.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3luimrzdm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wrbdwieh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fgwnjxuo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cxrcwbrj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kvkwsovf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hydpppzx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3uenmgway.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mfwwnawe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ivdayzzn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ztcnadsp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3aauwzlvi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ymhrqcpm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xmuytfjc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bkiqhwkd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gxogesah.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qtmobnnh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jnnrgdsp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nsqnhjke.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ncyivntv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqkmfqhm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gwqbquee.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ynuvpfao.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lohulovz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yyalolhr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wxaqihux.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zjjkbdrc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kteottfl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wnduwnzj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zcigklbm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3giwnedwr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ivppigwc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3pfyrwuew.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3swzbvwnf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3djdasxmc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bhhazpzy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xuxasaja.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3eyozwhtu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ozciprjt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sogdfolk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ekfwqqln.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jxmgzyiu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqsqewfy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3newmarsl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yapxpxkt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yphejviv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3klrpellt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3axrxbbqj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bnsfymcs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ztddoosq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rzteppsh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3surlvran.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3njfzxwny.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dahantmi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yafhnhmw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3heoehmul.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xzkvpzbm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3yhwzqyvu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qxxyfapr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xhcmrnnr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lphctlam.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bolbneva.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zfnvjyxo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ekkfgevd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bnwqlksv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3axfecnub.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ufubwcyo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3suhxpesw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3suhuuwaz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lppworew.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ywuifscp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pvlzbdut.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wkerzfyv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3tsqnxgyp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rpwgotwb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tqnbvzao.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fgcvddqr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vegecvou.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fwdfdxsz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zxkbocnu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lypxcngn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rnldjara.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vupfnmya.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jarbkvep.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3evqdwmwd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bjcsoifd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vftdxblf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mdeitvhy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vimehroj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jaowjmbu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iruqlbbc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmotqyvi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3eujbmvov.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gyxggory.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yzyhiqjv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hfsoorzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqlswrsb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3elagzchw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uygrgsmh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eemrcoxg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pimbqqng.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vzntudui.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gdslmazb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3osjddmlm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bqzqrdih.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3oqkvxmfu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bkvxicnu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ufhxhoxc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lujpzoje.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kxznmsvk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jruewsjk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3krsghhty.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3buovowae.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3usdxwqah.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bqnlysvy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ywjcbuvx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rxinuxvi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3abowjhca.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ghcfbkix.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3budfxmzs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ovhlsodp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qmdvnpjp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tlkvukvo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mejkjgvz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmcielrx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ntssagqk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qpqpsqns.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xrydsekc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jvifqyik.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bbnkvkvt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3okmvovhn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3iqiwupuv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qdwbceea.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fesdxish.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mnpoicrv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jvrphppp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sbcmlunp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3stlxqewj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nnfobxvg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ffepsttr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iigamqgc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dqhwqaqf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3orzveyid.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nyhcodrp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3sprsnixh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zlgpyyuy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ywyracgm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dxpjjkgy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wxfjbuif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ljjgqwou.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jyowinvt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kjciptbp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hdhksody.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3srfwtfrc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fetmuzgt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lpbrfcwd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbmezmew.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3faonhxjj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hgslbyun.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bxaggcbm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kpjriixi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3agwecots.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jcuzeurs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3pzkilvgs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fzlzmlql.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bphfpgzm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymmkfxlt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3drkhdhkx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lzvispam.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gxybduho.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cjdixvqi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ytvigijf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yahtxdgp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ebgilebl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zfziccpu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hvegcixg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3enyfqrof.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zfzzfppl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzvesswt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mqjceeaw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ymmakikf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rirshfxu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3msszymrr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3swrchyfa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3relyoxpp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3eppikskl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3cnbzqpxs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pybjnyvs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cucqxsjw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mggbptnj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vatkwsyh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mtepfcwu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xdjjonup.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zlktnqkk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3czfgcecq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qbavzkkl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiknorjf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yzgtvibb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dofufthu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbugztqy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ekvbiyux.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3szriffqa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yliqsbot.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tpyldklq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ckikitpd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cwpcdjrz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mzaetyeu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ezwnpmzr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hgzuikbc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vlyprbwf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zwzbyskz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mjxztzid.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xolxhsus.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qfepjivc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tromhuqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nakaqyrc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kppcwhlz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uedxrdrv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cooqmrnx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bylxbcjo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3opxplrlw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mylbojwi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zqrdpgur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pxhyulfx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ekoodrqa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gdalpwfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndrocgdr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mylomyqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpydejhx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxjqxrvv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jgrtanrz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tcirllri.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nllegbeb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tjkatimv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bkoxznqh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3koautjiq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvecqdwd.html


<!-- 参考信息 -->