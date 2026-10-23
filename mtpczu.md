代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ajbhaugu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hqqrxlfb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hplcmkce.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vkyzvisc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3birwsujx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rqpnebet.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jkhjzizv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwbjjnqb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3phzlissb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dwaqjzzc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ljcumlse.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pkzrbqlm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jgfdkxuc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bcqmwzjt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rejxlmpt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3iwcoexps.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tchgwmrv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bizwwksb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3itqbyghc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mhwdmbyd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yspvqmio.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zjxcumtf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qjwpjlmo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dwydwctg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hzbdhuih.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fhbriwvx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ycslpzau.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3duuusoji.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ebqdpmvz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qcvcmifc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wayhihxp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wiceopoy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eaeslmmg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3zfwhnule.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zoxxgwxo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rfgykrds.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jmaqsswp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3cegqhqxw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eiqygwtv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qnmbojzi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cgtfcvez.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ejlaexxv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxfmlatm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nluzmzbf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wssxuasn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gfaganjz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3efcnzjud.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ysjqgmza.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3imnqwpdr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tpjjpnhx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xhlkxwas.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3efdjnwte.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3eeqkbotj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hkwghlwv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mofnbvru.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjplubbp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fljiqees.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jkfoucnn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lgacozjg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wbovczxb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cjvmmrpg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3crebhdns.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewauplxq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3sxwbgflo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gowvdpto.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gisccvhm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xrmewgnv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xsjkyvfn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3oraulxcp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cygfjqfx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jtdbrrgl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3awpvnuqh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3owllzfqk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3abzxsrjo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rsrbmjsf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lwiaqoap.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tqllzokb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3silsksrm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rdvpzpke.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxqwky.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lkfhxssn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rnnapqsy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imtctvha.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3riqtoqkg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pwkexqnm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zfkszjvz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jrupxauo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dpbgapdc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3robnffhh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gdhnduet.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dubslpus.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3krkothur.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wjikbhlj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jszbiihv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hmkjnkzi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kcnokzlz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zxfhgtgu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gwcdcgij.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajbjfiuw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jpdziivj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ttkbyuuy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cvurjvji.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bnxwxett.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kxcbcpcw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3imbzeszu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3guwwrfpx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kaesufbe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mqatjjvo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3okhdoxau.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3taypunpi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pcyxrnzn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xvpiumsm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ieeacwlg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3owbytwuc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3onnwqcqg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ogljzrvy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ypogpmou.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xdfiudit.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3drkdcxfu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nqyyhhcv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3auysnpyy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpqbjdlu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rdomftnq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ytjkhdzm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zoievsoy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3balvfryl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xgeqnhzo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vnkyevos.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tifdwlog.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3knlgnpth.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kuumunho.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3beowhnux.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3waqejcwo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3iwuyzxmp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vhczeurc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dvewxzuc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3abxjiepm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kmnisobs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fscfptaa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pzmgtmzn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hueczypx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vhzfxszy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gcldrpmo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qxgwkzno.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ztphilcb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tlnujdtu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gbmzxbkb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mduzoafw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3fdtwuejl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3moytalbf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bjllorbd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ajmfdimk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3otcgkaua.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dkieownx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bbgkjdka.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ikqcrkbh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lripmdio.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mkmpukhu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3horkzmcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpdbwqwb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ewjdybko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjuqmzmu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3possanup.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3adtafyan.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbivppve.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ggbahcte.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3uliwyczm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rgurtfcc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3klinsqiq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fkblejcv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3keymljwh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bhpgmetx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3enrdsusc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3swpyadnj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lrvnwhqp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fylxvgxq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tftjdigl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3srxslmom.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bgpcrejk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qafnsaxm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jlsimeki.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jmxobedk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qlsqfrjn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tzkgguiu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hxdvzynf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3goxbbghz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ajcvrbia.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlfryock.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qghoktra.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wgwuount.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3exqwhnvb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3prlgdiaz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3sldicavr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dynlflvr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3uwjtmxtl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ncxhgrbl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wqdgraqk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opaoxyef.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3gjaivbrv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iomtejqe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gcwwukjr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3bwpeuotq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hwepyeen.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3brppmode.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dzvbtqkb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tkikzbee.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ejllhria.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fwxaudiu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bxbdytvt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3etlaghew.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3igocnbxs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lwecojhp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vvrzjlzo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pbtoaczp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tyehbhzh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3udmubmvh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3szorhcyj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jaylqzki.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3giuwletm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbpqudtj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kjuxkvsd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jyjheepc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3eydsrnpc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mkoqdgxa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zyzyykia.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gmozaqeg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3umrjbang.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pwdwieel.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lmzeyesk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aotuvtgp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3autdnqvp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fpxrwfbq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zplxrucp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qpnqakcp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gxlhpvrg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qowzfqbc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rlavyppy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jdfshffr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oxgbcrtx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbadjmii.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3njelgccw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zwkjnswf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nwvzitec.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tjbwgihg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ttjpihxw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hksmxpld.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mccqtypb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3teerryhp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3egyrghuk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3safxhvsq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mbakejlj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3eunbwkxy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qaueiyei.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lavyvdlv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dmgbmikf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3evqnyrzb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fivaynzo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3akzlykoy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hcbxrrup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbhwfcht.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bapzwhtx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tteubwpl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ilebfrkb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3znpadnav.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pusgajas.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qypjtimd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3aycfkdvd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3srvflpka.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3giecbptj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cuyqiyru.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yushipst.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bmlhrnho.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jerdgfqi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3igcgnppo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ddfqwnug.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3abvdbztl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ztsflgdz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qstlsigp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kufczrbk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vszwribk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3glzfsetd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3idxnombw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sgznupbi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cmhilsbr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hkjaxwqd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3cdyaqfdf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xsoldluy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pipyzawy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ptljshlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvbafsxm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ntjxuppn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuzooddg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3onjvatbt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cgkidjxg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mulmvudq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3aedcukud.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gilzgslu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qjefzjga.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dpgcnnsc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gczrpvpn.html


<!-- 参考信息 -->