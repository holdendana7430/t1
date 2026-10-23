代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hwfkmeau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luxgnufu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3whxzksce.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ubolgylo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ehjuoiem.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ezepjkax.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lcsmbudc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zcsjykuc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yjnxjznu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wuigbfsy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tqwgjwww.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yshutahj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqbayyrj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dfootlom.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxebusnd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gmcvabaj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ulnxbzuu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xsmlrhij.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ubtjtaqt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jtgifwrn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wzxgcxmu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eqzpufok.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ccmuzkam.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3niaggmqd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3guunutaq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3scxrivgq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tbaihovv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3cityiffl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3sbavyywd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mdbfecje.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wumzxjgf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qfpxybjv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aotxugla.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mmpbetud.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lxcufldf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dglakpud.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqrtxigh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lasxvngb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3punwkopq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3uddzmsfo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmaapeii.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rhrakxyx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3unxandmx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qymxopxj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gpmzqgxx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bltndtbo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xjplozjm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lekwbduc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dlmnhncu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yqykzizk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rfbvexzi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qhgazhlw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jrnzaknh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fktoupic.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tckmkoor.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vuqynozk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uppssrfk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lkdbzhns.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cgdbxedt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iegfsyox.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ejobfxxa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3swsrzriu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3timtyyhg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xevuhvhf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3lhyihjuf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ozfqgebc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3csfabmkr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lcxniupw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mmpjextb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ezrsgksx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3drmocaqj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ctpvuyte.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3okvjvufb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jrpqbnrd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zdbdmtdk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hwovsgac.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uyhldykl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rqyiaozg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dipakndu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbbzteil.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3chevdojd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nkydyqfi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jrabxsro.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ppbngfcs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eqrhdevb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3atfjzxtf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3aiosqsnm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jokpiwcu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kxvupyrf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3atdsokbs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uxakatjn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tibqkyxl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ppowpymq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pmwasknz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3varjmynu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rioeeiab.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cbtvkfno.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gamdedhr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lsqfbbiw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hnnklguz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kfurxcqm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ekgzdozs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cwegubsd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nqmgqfcn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mmtklmxj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xenffbua.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3liigihpa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3edeqipfa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tudwvhkf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nhjzivrz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sxrannkf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3iqxuczeo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bzogktxe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sppqddwf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rkcbckwo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vnejhelu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3srwmtwns.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nqldgdfv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bhilbcpg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3yqbvplnf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vskeivsu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rhvwvfyn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3blovrvir.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3caikgrec.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rdvqmyzr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mpauhxgx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wstnhohv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zzquatlg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qmasboxb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngydrtmd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dayfveyn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fdhsiczy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xhfckoqd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hrffmqrk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rksixmzb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wiufalhd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qxyoddqk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3yjsdgakq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3izybpbsw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3iarryzaq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3bucobqgv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vjrsmpfj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vogcyscc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ygjonbsb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tkdbmmjv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3oihkxkvg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sidivlpr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ttbljajq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wgybkjtx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3noslwezo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uzhcocfx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ikqwnrkv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pzebzfre.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hjtuxhvy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yjfduzmk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehxytwoj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qezcfokq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kklprotz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vhrbohmv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nsiberjz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pfrlrzat.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qqcdqgzj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yshultve.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jegadgse.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pgixssah.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xcwymtym.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3iwopivoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzbgjgjo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3oisksdsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3midmffiy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vjmolgqb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zewdrbfi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjfjoqcb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tfhqydyd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3numizoqo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lrhqrubo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dmkjlsri.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qfxipnao.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ltpklpnz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hwxzfihg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmasgvcx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fkxtxbeq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3whcbnryz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kfxxhazn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ipyqgqkg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3lxmzuvhz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3brovgsby.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ebzhtnqr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ikheoloh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nwjawpdl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ekesyxwe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xpqjaokz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qrwxgunq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pnvfiaqm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rthbiqit.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jlxblnmn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qwfpucns.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3sutkuhjc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3plrwcflx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vqpebzas.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3clkxaaej.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dedqhotr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3khrtkexa.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3chcvpvmp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oestskvh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fpgdqtlw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dluvlryx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3grlgmpld.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3acioeqwy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mvuatleh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lzpyehat.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ztmwzdwp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fszkpxgr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpzwgj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rvmrlvva.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wywzvihn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qwmrhucs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gdmxhqxb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dwfuuufb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wownibuz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ivnwsyfg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ltyiarwe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wrnydtsw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3eiqlrxoz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dtmlowwu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3omojkrxr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eocdzcdw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cnpmunsa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qhigkdbm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzmwiuzo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fndxhbyp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mxodkmtm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mfmyyadu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zrbzqmxg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xykegmau.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3awpbnbfr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cxtwivmm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khywozgs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3eznhnmlb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3skrdgvlo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gmapqpqy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3roenmjwk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lhylyapg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywmwshdy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dnztqvqz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lvwvlnsw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3seperutg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eszliayl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hdhtquax.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rtbznpjh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jnlguhmf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3leutrcxw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3goqijvhy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kcufaosj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vxvtbnpi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rbyqbgta.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bwhxpabs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qrlkkzit.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wievsnfp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pxjvhutn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zzqsuiva.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lahqvxtw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cqbdoxed.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pvbxrwnu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3djznhpcz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gqcwsqzg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kmhnhngf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3efgulnnd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hsinsakt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3swmqiyfj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zaxwxjgj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qniligda.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gcauvlrn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqzpxsyg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dlugcfpu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kdgwiybd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jcupdaui.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jzbcuixa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xnusxjun.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3luqozqhq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hluirrgv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3pqncvrvv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cwhzpjlh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3oywjlywn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rkwtqtrq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tvsvjomp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pfetisfr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pollhoji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgqjyzus.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bgpsawit.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mkvrrqdi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3byuumqmy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqnlzaz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cbejdxih.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mmlnwsqo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gccmyxgj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3obpbatub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpseqghz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vjyrhcts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfywmscq.html


<!-- 参考信息 -->