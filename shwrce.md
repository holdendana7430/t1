代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gecobmie.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yxyagfjr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2prcvluwq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pvjqmdwl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qsxgbtrg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2blofghki.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2eetbvokp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nfltswqk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pubvgifp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vdksohqi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yqsrqrjx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2owoqifow.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wygicvxf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tipfgove.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jldjynad.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jyqlsyad.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gebwnjrp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdwdrdno.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iywtibwk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kfvyiwin.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2osafhtgh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2eyvwmuev.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gyrktfwn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aluahkxd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qjdrmshb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kceudssj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vjjlggzo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2extohoeb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wufimope.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2foxlrgrl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lhnuimcc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rgfqxiik.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qbglcdfm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uopueqcj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hqiwyhig.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lfxjvjdt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rhvzbjqb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aaroaxxi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrrjuokp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mfxzjott.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xwherasy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wkltuggg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdtblmsg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bbgimtya.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gdlbuhei.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2khtdprts.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lsyeqavx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2arimjlzc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wtitkzok.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2iorzmyjg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gfacotcn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sgvpmgbp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2uhpdeuju.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2suwzcgqv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qlqfpicq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uxeifhrk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2slaqfqwa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zyjscuct.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mmvttfyp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rbgfwonb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ihukciem.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jvjsqzlx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2obwigvur.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ooxckjzi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zqzokvhs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2csjesbio.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2alovdhqf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2swdmmrti.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wsnhilgr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gtapwezj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qkhzzmdc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2guaskzda.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lqxrertv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qhhccnym.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2sloqatwf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2smfwjvrm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jipsprur.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2wwkvxvwf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2myjaboey.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kcjoutsh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uqckinrw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kkoiovdn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oafrwxll.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qbfbvlcq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hyyoahwk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bnrmtpfp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ecqdyemz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lnnhfvqp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tkqxeccu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jhoxjthj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2etazabqv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hruxbrcm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yesmthlm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rnsdseim.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jggzjfnt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2dpcyukcw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wihtxlmq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ojjodfcg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qrzhhbkj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kubxdnvu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zetkcigk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2adxalkhh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ggdecjax.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2oufoctuk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2udngtumc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xijslzyq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ahygkpsy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2himyzxnk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2anixdhzl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jdmkicte.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2exfwhopq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zmohatij.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2stbisuqj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cjsuxxrc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ieclugqq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wqhiiutc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vjkkihff.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfifawts.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2allaijxr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2uroefddc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2tjqdksrh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oqkrubml.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrrpxdo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vditlrnd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uerzttfz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2exmooxnv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2koaphhpe.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hupduikw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2eqgcunbx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tssncssc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxbkpukl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lmppsroh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jwuxyqhz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ygplbdah.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2enerzyyu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qpcnwwbl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bhkussxd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pjtgxxzv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbyhxxkr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kpxgnoyp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hztyomum.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zilcxheg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zaugufik.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ntgrbkkw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qxbtzztn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcfonaco.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2umuehfwu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qcszseel.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ljhhdinr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bccbzthy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jnmheizl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yfijpbql.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ccpdmtca.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pbygndfq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qousujde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asspsddd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mzqbomad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbgcokkp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2chdjhpip.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gveimqow.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppxccjda.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sthmhxgg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wktfmorh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xwcgdbfs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qdyvyfgp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uegvkejh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zxsygvrq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2omyqgwmu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2iwcowyzf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ftomhbyz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fhsgxkpu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yvfqiseh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qqbdckud.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nfhgrins.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2aqbvqrgf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yojwbzym.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yrpitsua.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cqcxxlqz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bzdgnxkk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2szpmzaku.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gmlhbgbu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dghteojf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2umnzjaze.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xzhrdlvp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wlfqstbq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2puehoqpr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mrhjwjrh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iiuqbztp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2unqokwus.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2defffkrr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kfqdjany.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wccwcrdd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hpsvfzba.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qupmnyzy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ryowzhda.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2buqtpckx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tkrjxgft.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bkbordls.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mvcrmyxz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yxzjabkr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qkfyzgsu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2raftjwcn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uqayzqws.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yepppssk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gbscsoif.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hhvcvhvo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2weilxepr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gihrurcm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2txtpjctk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jqdavujw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cycnrixm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fdjmwlkk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dbbhsmnw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xqvnqmpf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uyrizlgk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yyhiawly.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2sirpedao.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2npnhmohd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xwunsarn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kxxbeopv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kyfhswjt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2endjdszs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xnjwnrlh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2btkvcquk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jyrhreiq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rsuwcmkq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2lcoipcps.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2yxabfvdq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ogkefefa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dmzskqsm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fwndpmnw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lejftjqe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dvmsjrrr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fchwsgln.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cpxlguss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kslhepmk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pwlhcujw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qwxovrhp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uvwukymr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zbvieyzd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wdoffnxz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ebnkqvax.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fnpuutku.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2owundlxa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbfylhio.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2evjgzpuc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kdndigru.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bqvpnbnq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2drwgmzje.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ndpotxcs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pihqbrga.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ykgcoqpm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2uhrwokcw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lerydgjm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qzeinarp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2clwxnrpj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lwgnnslt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2siglirdk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2izotaagf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2meohxzus.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2exwfeets.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2anjliwyd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2shetltdf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cthnnevt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pbwznebe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cttoiawb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qjrxtrnm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sjnzgkgz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cppngogn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2tvchyxak.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2stoxycdw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vciosvak.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zjksmuok.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2efplkpxs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zeyaprya.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tsleqzmf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwuisiyh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ztkrfoha.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rxgzypan.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lwolqpxb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2liglbuve.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qowbckrw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zuyehlkn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qeaifezg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wjwresct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euetnibq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uypvglph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbfceohh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vxwlzfgv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uaqzixne.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfoqpkye.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2igrueuwd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2blznjcwf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cltkewwq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hvnjwztk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xiejyxty.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tipizwji.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2endgypxx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eosckxfo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gpglmhyp.html


<!-- 参考信息 -->