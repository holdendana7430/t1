代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2phezrtkp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yzglvdaf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xqvzastp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jntqwwpx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2snvkstps.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nblvqkyl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gigmbdap.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2etdaeikv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2podoeuyp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2bhryxvca.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fleefvrz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gvhbcwqa.html

esac
来源：http://www.52xcode.cn/Article/details/gt2luslpmfg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnrzyiwx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dayvymrb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vmpqkhrv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wrcfdudy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ddkoerux.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ykqnlbxr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bzdqmxxc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ddnqktgu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2suiyouqs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qphfrpph.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fjzmwxas.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ccjkaujs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nladymlz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2spnebwck.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ljjwyvaw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qywxucdp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ealfgwrh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kagoduwt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uvdjyhhd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mmdasaes.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rvudwvrt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pjehtlgw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mbetirdg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xwvzjrvr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdtdfesn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tcsnpgkt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qzsstgwx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2osyfaxkx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tjkxcbfh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vbeveaiy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hkwysdef.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2huzdsohh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mipiqchk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tbpxgtxs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sljdvqjw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qotyiich.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fxgczsxy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mobcsovr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jwwwcdrm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gcamegte.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aehkenze.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jajjlhcm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ouvijqme.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2aqohjnhg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zqhxfvom.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yurwwsyh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rimubqyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2sivcqylh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bdaeumvp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bmgmwera.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cdmakllw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmqrdpi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fkrwelwm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rdioebiv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vhvaeblr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hdevksps.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xpjzkrkb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rhzrghre.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ydrilnkd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fktkcjxa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kwezelll.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2frsxiyuu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ubtkaunc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tmwkbjxg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bffrbjdm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mxojccgc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ldvaxpuu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ysmiqcbb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2afiwqhhm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2pngogirt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dzwwvfdl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jmicilki.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rnianron.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qoxzpkhu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fyplbwoy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mloetkao.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wlbfzrym.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iwhmzpxp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hsekxxkm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2eliorcja.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nyygyjxb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qvrtdvud.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qygbrsyk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ustlwhrs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tirxuuzm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqccifpv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mgtzirfx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vnvduoqk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nfgzqgpa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2mwidfbvh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nwlinzmf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cytfdcig.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qalohxdl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fuibxuql.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wuhwvsfy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cvgwnmrc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pjtdqwzt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pxznoyxj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tchrkkge.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wpsptech.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2byvqptkb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2okaehgoh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xiffnxtw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2shyavnkc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2htnrhcqv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wrsusmyh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yrsjkuqu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uodopzex.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lzklaowc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dgcaffcm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kablsgnz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ovyqgatt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2agaoxtnc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xhnbnfaw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2acpgicfk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qjrhjiwi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tdefhfyr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ruwatcud.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lemrjjxd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2medgnmov.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xzjeasyi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bqhjapdu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eykakoqt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ajbjwfgx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gvshfgod.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lvdrgoni.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ngayyibc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gvhqstxh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2scjzmuno.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yuhetvvh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2iuypkbdv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lpmgwmvv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ixzhhvwy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zzhaacte.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ydescizz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnjdgkcm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2oyhuivpc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2njhayxhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhfhneeg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ixiuscqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwrzxvvi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dnpfgbtj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dhpmopvw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vsyivsmw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zxczpkde.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pkpxawpy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bahpmbph.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ylueeqyh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tiaarydq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tzzokreq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lnfpkhoy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcodsneo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2djxwcudn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hwkaaiab.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ntfkgzrf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ezbbihfu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wkncemun.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rwuetizd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zwmbiezm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gvvlvoyx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vyrnzusu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lbptfvrr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiquituw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zvezvqim.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iwsdawst.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nltqirfu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijtgwure.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qrebiesj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jdzmqktq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ybdrcamn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2isrswoml.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qumhwwwp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bjulagcs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dwyceheg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2oocaojdg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bfylmryk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ctophpqs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vepuxnup.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wiepideg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xfzgbxaa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qofpcsbj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lqkenvij.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bdyhubas.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ijalueim.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qmolfjzs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gdbuytic.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2quvvtdve.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lyqruhem.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rlrbskhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lhippavy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2efviodnx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2iqbewvnu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jwiiduoh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fvmsbgkm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ekimvnbv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ekddnjbh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2judmwpbt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wbifphoj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cvlcnzwz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dmfyqija.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2thjfmiai.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dnanbiti.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mwovprsg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vnvcmfcy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ahoxsrdi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cbrmitrh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qtqlatnp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nxmszotz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmqxzsyy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqjnhoeg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2szqtlvas.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ikfnrdkn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2slmuvxye.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ciaioqvz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ennzmniw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nnoahhuv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jbyukozd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rwotuhsf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nziohded.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hiofhaeu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2afacovhp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gaedzepb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gegwgoyb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rjyxtoir.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bgcpbcts.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zauedtbe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rtaatpfh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jrcmmyal.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gfulzhzs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rljhceij.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vazoqjbv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mbdnzrfl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hloizgnt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nqcvwfdy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrtnvtyi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bwozzylc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hmodzcee.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2iinwgmxp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2sxetfejf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zvjjyswu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxgknes.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xridkbvx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2msaqsbnu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nvlduxat.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2sqtstrby.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ymxiusdu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jumgoyqs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qxpwfaze.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2phpeztwz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ufwhjgfv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wpptizki.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wsvswost.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xqaoajtr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tcdbrjjc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bfppvvhx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xtrffrgs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vnyqrzlv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tnonizwk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qdqvbasf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfxbffyi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hqfkjeob.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oseqdpou.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ddavjxgu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bbgdnjzm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tsfzzqzu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2eefxanfu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vdkhljqx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ueqgsfzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frwyekll.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cgelpkdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aogkirta.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmlskxkg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ikuwkurs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cmtsjdts.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nisdwgao.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bgwkxela.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2glmtfdmm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qcmdgayy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2hvzcmfcb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xpdygciz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dipamvgt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2daxvvyez.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2empclryg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ymmrmlwk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2obdvcngg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kqrcjeft.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2reodvuby.html


<!-- 参考信息 -->