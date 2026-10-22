代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yjrlpplg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bfzvlgep.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qxslgqns.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pbrfnuls.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bjjngcnz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2baucahga.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2caffpokx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pzmwcefq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2oatwskck.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdrdnpwz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jokopxsr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzehyufa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lnndcomj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xtjjrxgt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vidfrigm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddjeilbu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qrxcjdnz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mhwggwfn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zvnumjbv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zzuyvrno.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ltauarop.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yphsnzfw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xxynahmg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qnheyiky.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vzcbhzeo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uinqaysq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2leqwlrad.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2suorjrwk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2feiteacy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vbfwqjbs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2sawpgjec.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qeyessqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xqmtuhdp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fqlppvvp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qazdnjuc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ivpmriag.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2utiwvxfz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2kgnkkynm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2udurpagl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gsjmljem.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2klmhveyu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nsnggefu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2putsjnbd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfosyrhf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hjhnqvmx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sojtqpdu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xqsomcpn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2woqvztiz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wofqlsde.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mwctyyiu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2stmwccap.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2svylgpva.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xxnioufg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2flovfgbw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2siqljlbn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wsgkijlb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lmdwtspi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nbjdvbjd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2aoqizwrd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dfidqaaw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zeedpxlr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2eqrtepoa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pwhzwiub.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2twmsysyo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sntmbvnq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gmvrhivj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jhhaxwae.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2uukeopxs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2otdlurcg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2funsribh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yswihcpt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2psfaljkz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2icvantsa.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lokqidzg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vbuornky.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2akneckyv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cwebsfzk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vjixtlrv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2evkzlsdg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pakbsurr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sltkzrsj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yrausqkn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dmnizgrx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2devhfeae.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2anjkxhbm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rlqghhtr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rmflttms.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ypjyhhns.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2svkxgoku.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lfcyrnau.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2srftoimc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2evomixhv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ehqbjouk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ivtscoir.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tgbjtwzb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2uxrulgwv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cciwcwlj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vgmgftas.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2auzromyo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cciwlzkf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zggyvsoj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qytzezvi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2sfzblaqv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vcelwvkm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2shxdekal.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qdzopunp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nbiqjtnt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2niazayve.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bicwvsti.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vibwdkvo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qasesrsc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2avgrlmfu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ypdugici.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ooaifgdk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qbatihhy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bkvrcwqv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hlnxguyg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ttqsmhvq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2muvdypxx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cazxytcr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2azmfpoum.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ehmjteac.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2avtggdty.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oatizuty.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jcwdbxus.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qdekfnle.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pgcbdsno.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gaovcjhc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pewqkljl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2leepzyar.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xycxxigr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xtwnhmmw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2langjhqb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kiabitvf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fhrmztvr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rjwwourp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jfnefxht.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tfazlpeo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jtxevkbk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jhexsgea.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2prclsrvv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zldsfnuy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2gngoedov.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2auhksaqh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xlzerwby.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xoxwrskp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ocsppnxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxyqucur.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2isddpwkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmpexrhi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hnxjxhhr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2sxwapqrr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fvdekgfb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2soiortdx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hcvrlbxz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lmzsdexg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2oxypqgoa.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tkipfitq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jqloatij.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fbpppruw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bqnscwmx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fmnhmknq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nozrunzp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2aysazqpo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bfbitbdr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ixnztslk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2oaalpivo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2cgsuzjtv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zxkdxomc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2quprjycv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vuuxylhv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wtjijxpa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pragpalu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tpprnmse.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vtbegafa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjhhgamq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ntybhlwv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2feccyiqf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nwxkabit.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ebfygmaq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ytchnier.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ejeueamw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2utaujyty.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2igxhhaav.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hwcipjvx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nslmxhvv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2irshtued.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aveowune.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2elnpeijf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nopqxifu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aqcrcelj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ezvszwsd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2evlpgllz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ojthvtve.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rmkeftjx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pqbkndvx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xdnjhceh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fejxwaet.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uddctdel.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2skityrib.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nysetlot.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2daxlihlu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kgmlpxew.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2giaaetmt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rcgksevk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yggdvbli.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lfijdokd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jgzvsvwj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bduhovgt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vepgbfcq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rxborzrd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2sllsbtkz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2sqhwdgap.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rosfjivm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qtgysqun.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sunozcqp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cjpahwym.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vacgzjep.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rocdxkvb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kaavzfcp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yurwypzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nirraojx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bwkrofre.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ehqesyhe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2inuzrcft.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ykoipyby.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xgfgzlcy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2abhfaxmn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ggdicqdl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tpbkrbzk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2eulsbkbt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wolzwxob.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gcifxwyr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ynhpagwm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mukxwmru.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zhysjgor.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qtixzeqq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wdmygbdf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2djmstcis.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fvyzimjn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bovedumm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xmgqprbn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2naycadhw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzleeziu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ognaqptx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ptwacqcl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nzhsvrwz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2umuzrcwl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gpqsrmux.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wqwigbuh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dwqjrfui.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2snorchwb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2waagfcft.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wqkmovvf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ykyoipbb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gtnuvzmi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aoisdxof.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sfkgdeoo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ppbhnirx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fcyfmgdi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2epbtnkaw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ezwszkff.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2boggbscv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2inqptewk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gsfnfitv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ehtfjcir.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rxdwfxxa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2htqnkkho.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cyjhpdod.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2icetwodr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kgmsxjjw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tzuimhqc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pmmgccml.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dvdypgvp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2imlcpjuz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2omhwimfo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hdazjngc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwnqxyvl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wgmuwcbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqpxhwsj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zewyfhtk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2numgqyzt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iwhvfazu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ronrxiga.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rpcmxmdp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zxgrksbr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cnukvule.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xspidoko.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qvhlqltx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2aakcnxoh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2libuzgfj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxzgaljp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zjpfuvij.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2canswgxh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aejishjj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vbgknbeo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rbcblscy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mmemzohe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xjlayhmk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ypcncvpw.html


<!-- 参考信息 -->