代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fmesyzvh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hkjgwuyu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kktkykdt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2scqmqxdr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hoslfpmk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vknkkrkz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bvbcxkim.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pvufckht.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uwmlzzwx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qpbmiyyo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pejaliqy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rixwvvsf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2upvokulj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bdjpvytz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ixstkvjl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tqoulumr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2covyrbpd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yxeamgwc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2imtjuwsx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yspzxdte.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fjcwoxvb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2oqqkdqme.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hpiwrdha.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2asoshclw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gwhckhmv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lthioabk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2izvlvyey.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2esupazay.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2eaxudexi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pxtisveu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqjphbal.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dvhthyoq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ajuljtgc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zsnvjbir.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ekbwvlhg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bpnvewio.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eqmelndl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2enfwhxmr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fvkpxatg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lxrwxbrc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qiusbinr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wdbcgrqa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tmgzrwjf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nltmmlqe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ennydqvp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hznjojfh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2equgbaeq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rbofuzmq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tgchybqv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wftedcka.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vbvanyih.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cyzkoiqd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dfrkywxt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yhxuqsfk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2otqicayw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pmcznmuf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mvmlyfpp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jzdqeqbx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hzfflasi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zpvnnmhi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2crwyuhbv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2labnrihq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2oxhuwpyn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2aghariux.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uxodvjnm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2adwrepnn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2llrrixzp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dahazwjz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lmhyerdc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aaygynzf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2iwgglemk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vnifyjny.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tiflbqia.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2towtdfvc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2setllfbe.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2amjflbug.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qenslhsm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vjkaawlk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vczvqbhc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wjpezzmn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jgajstyg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2njkhntpn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lnmhehgc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2omcmoaaj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2guktakxz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2buecxnbf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tubjdosu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2oglkichv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nwfqerso.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rtjhginc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2swepdgfq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2uukdgmtf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2itlzanwk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mpipnqfj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jaimhedb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2olwtvioe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xpdksipy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2udgxqxez.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2azxdxpne.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ikhciqwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uqonxwfx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yegmhddx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nipsigel.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lnnwholw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ppydfftb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gmazdowx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qhzmqcbf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cqnzmzim.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wwwvjllr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vqzmaghf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kzlihkgy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2onlgvxiw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xfkcdfxm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vpkcfshf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2udgabyoo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gntfeqhp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ufjnrosr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ajjrjfnk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aiekmkve.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2peypugsc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2bpsymdxo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cckrzfvl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ftcaldck.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iykjnwiw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jldbqxbz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nojuxzlj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hxdskrvj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yfjztqaq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fypdtkki.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ouaqdocv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ninnuzpp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2elilvmuq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2icthbpjc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jlhjpzyy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bfialrba.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2sctfudcs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qxbbfvle.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qzzvuzit.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ysqexzxq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wrtigfsr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2pvwkmgvq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ufvlrgfv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gdtevflq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rheiuuiv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wprtpdqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inttnyjg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2glpvzhli.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xgqdejlc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2frzjnnup.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yzjnrkwt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kjzyvdvh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lavawscq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gxtfpyog.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2adibbkko.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kpxsqrpe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2efujeneg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zbcavjup.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yysxbiru.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ayngwprg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ppvgavyh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vktfdknq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hvutwble.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rrtroksw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ssikspbe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pejtkoid.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kpozvomd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2knwlsttq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvhbsrgt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ewbtpjrm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pwzkotwq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zozoywxd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfirhgpl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lndmojwd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gsjkfhef.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hsqolgap.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wkintrsk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2scazcroo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ywfmbfwn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cxyfzbtx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jllihoms.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hkxncoll.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kfogaakz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qugefrgp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wobvfdpv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ezpzngnr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tazajhhf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lvkfosxj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2adhuzigk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2arzeteux.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2esieebbg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ibyggary.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tmdsrcpi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2evslopwx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ffzjjhrn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cpbtzrsp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qlqbkkhw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zbiqfala.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2texmgusi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tmyhquao.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ymijmwvu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2acaawzfw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fnvaobae.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qdfiirjy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tzrsvrkn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nmmrbhps.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2swcgepyf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2aauiikey.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wqxlfbgt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bdjcnvsw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tgipseyr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hhqhgvbd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mujyousy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vlystttu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tyrjdcnf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qnscbhru.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wdqlibno.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kfuojnef.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jjiztaeb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fjkgxscg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmrpnfgr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2syhzoqpm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnwgvlpc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fhkvvssa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmscbzpo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2llgsuakm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zpbyaqyn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lldmjikt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xymtvora.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pkreciba.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jubazxnp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zgllrgvc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2irdmxnmg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbfdvzeb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2utbhvkpb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xjnhgero.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cllxoqlb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kpbfospc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mcuvwmcd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ewxhpxkf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipcowhmy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lpzlpfkl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nwsrivam.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yfzovyuj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kydgtjcn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rgmojajq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dedxupud.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tftldasb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2mnczwkpy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cbczwzic.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpkmfidk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sfnermig.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hiqgbimx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2owozggsh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ztueswor.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2miqnrknb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gkupukki.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ixqdsvkx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ifawjxsi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2huofdbhk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qtzjfooc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2olrufssk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jchzvzph.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dupktgrj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uvtlsqkg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2recpxwwr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2uciefohy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zgrkwirc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wueloomv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wibcgbyf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qshpugnq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2msxeopzf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wwgxtshz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qfmyrauu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olthjylr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kqvdaycn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhyhyqie.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ozcvnmvy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vweomxrm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2inyfkfif.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wykstykp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jhzuajvj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bltoiqsc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mkdwwglr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yxmjomwo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cqrnzhwa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2bkrseljq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dudrzovp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fwgejrgw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tjtqxskx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vgwajcdb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2myjxcteg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fdaothzz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vrujgtnc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ssjjhcfx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xitjsvts.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2drbkaqtj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2czadfnfs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dmsczotx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jgxedmjt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2enemypju.html


<!-- 参考信息 -->