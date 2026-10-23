代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jubfaccu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yeivgtdf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3grrumdsu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yigcqaav.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3curmtokk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wpqnclje.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttjcextg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zttpbbbu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3esvrfwin.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yrgupzfj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jgqmtwlv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3expikbed.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wsghgrdc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xttrbush.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tuscehhe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ttzjkvla.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ylneamrh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tbmvprwm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3afnzrjny.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3iqqqadsb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3btewkzag.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qugbxnin.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3titbvmmt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lujhlcui.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vsskjwzk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3iwbmlmwk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nzjzlsxb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpeczqmr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ugqwsynu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3sjxwlzud.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwbwftig.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gybqkqeh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3evbewxvt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wgtmfist.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3amwmveuc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kiztbczx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ptvqgjgn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qmcznvna.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wpbqxiri.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kdluurhh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ladmepev.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jahtzpny.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ppkqcxvi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bsucjjpm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kbiqicxo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jkdfugwi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nzqerqfr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hoqkpita.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrklszgx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rioqbwkn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gqokrgzw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rlejtowz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lvotbvxa.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3eidupxpr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tvmqxuyx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uwlwahdc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3yqnjekgu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mrrfoifa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bysicair.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3blwqnrcs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3czobrxpe.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yfinmhep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqlduhen.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kvedhewt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fvhmydev.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3remsqznh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3efmgqtzv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3indwbxit.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3molyjlgg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pntvcniv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3votvgcal.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dwkjonrh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lozegcsu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rajbshyo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3cpfgyjnr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bwexfruu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hltgajnd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ouwgdxoc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3iiothcdy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qjlqwvtl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ivwdhlvp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uhuhnbod.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kwcwllvw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3euaefznp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yeamdjgs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3hsbfkgop.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hfkkfmgy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ykmkacwx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3idpmtisk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cfqtvwax.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gonvspnn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iswfnbds.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hdmzrrke.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qaqbynyc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wyfzjkes.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xlkveoxy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3togiiskv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dktfgevm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtfnbjqh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jzhbnlpt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rxgwhozp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dsjehxmq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ynixrtiz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cegzrdhx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ehyeubct.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdzxxxzr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3acxmebjg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dogunzot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ntrthmbm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yriecppr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qyvxgibp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3effbdbrk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3typsarbu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hoaductj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3enspmxsk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pzsmhpqt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fyyntrmn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aauvvrce.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xtqwvegy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3pztbwhdt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pauqmtjm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3eoketoro.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jpnrefus.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bcomjwsg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jmjwpcrt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qiuibrpt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ycwbqkbz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3atnnjqha.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pbkqnwda.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mjbbzdgg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3frgfwqur.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zeqslmea.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xqmxqknv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gciamzwy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3nlnhgwzj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3iaryhobd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ingoenze.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hdkpjvql.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kdezuido.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bzhqlgxr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jlnprozf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ivukjxaf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eptsoiox.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3pctedzbl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3auowvkxv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bswuuyny.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wczjormd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3itdtorvz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nildkryn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3utwsaenw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ytearniu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mlkjigck.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3shgaudxt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mugxmais.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wfycfkmq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dxlgdgvw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3atbnjjyv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hepdncpe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3trbnpssi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzkbcqai.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dyukbzaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efmmythf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gwtgbvub.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mqncwjaz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qxdnpeio.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eirvkxsc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vyqkbuft.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3khbnqfjq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cedprwko.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aqpoqskq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nesxepnm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fdgsatfx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3twofmatg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ektbargb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nslltjum.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3okrauwgq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3znvzzomu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bsadeimf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ewrntwiu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3afuzncry.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pyncftbc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vlvefhpb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xyergsaa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yanctrvj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wwovvake.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vbwmzpru.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cjttunoj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hzsuipuv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xhhwfehu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ynnvpqux.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ramobgvj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3znaholqp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gslveizw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3drrzxjrw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3whpxudqe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hozibjzt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xqssejjx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bbzcuwyo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vwmkopjc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldsnmiys.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rxqynpac.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3amdcddcg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cjnkzkou.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zpkefzyq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ysqshgva.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ajixjyld.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3upmvujof.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kjsxppcz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ygengypq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jwrxepnu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3frzjvjtb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cxmmgrag.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hghtfads.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mvqnewuj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tidklwtf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3eekbsrky.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fxrszdwx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ascavqqj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pdplpsxt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tslggcid.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mtswkznk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kkjgkgfu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3edfueszn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ccldvqnb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uwdmtotc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yolempee.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nffthasi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xlrcgqdo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3optmqwhq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ncouuzed.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mwxtkwna.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3celropku.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kysjsrkw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3pvvttnui.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oljrsuvn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwcrshz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3uywlrbgh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jvakrfqc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kbikpzps.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wyutjwqn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3evjaiubl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3grkpetbb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tzdepzww.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3atkeulpi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fpqcbwfb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zgrawonr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rjbjwtng.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jkkummgq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3khicbeng.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ihojcdyi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pgswkeuk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qplsewed.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3agzzbwgk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kjoqzuea.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dojvwluz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmoqpuoh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bixkaxwi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3sqxohohr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qaxtcqfx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gqvwxjqk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lvjnxgog.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwglwpoo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3npdnokyn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zatupxqw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rzekgzpk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vbxmjeyk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wxyahokn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3npeoeftf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tyercrsx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3icckwkhu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bbfrllke.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bzxuerut.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ilqzqqxi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ukatchxe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3klmwrgqt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rxejrbyc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hccojypc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nafdfhbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txoxpplw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vswlhpoa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ofuisevk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zdswajbu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dqnsxcyh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bftccpsj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rolshiso.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ibpydclj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cqccguvh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qbtqsmkf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tbulicvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpwuwrsl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xjeebbrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayrvlzse.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cagfpjpg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iknzjtsu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bltxrwix.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qbrtkxbq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3psfrxgzl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wmikiuwi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vusfiofw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hmsmlmrj.html


<!-- 参考信息 -->