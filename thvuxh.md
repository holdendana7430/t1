代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zrhugrfg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tagwzbpe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fwnxsueq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrslsxkn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3flhqhbfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eckvdjpi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kcwdvaso.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bnixrsdp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tzwucoqj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3lqhioilr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zbmzmdne.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ynyrqegx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rdnvcana.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxdthqcc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3trqkkcwm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jbhqqbkm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bokygbox.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vezlywly.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ablzyfui.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3oychrazx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xuddbjdw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dhbaibje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3izacuevv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yxvfzsir.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nxrjhmjx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3iwlgvfsd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ylqzwxkz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nmzneizf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fngnmvid.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ihchaben.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lbovcqac.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3oxuxgktc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jnsoadas.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dornfaeh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mtcwlpfm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fmrxyhqv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cjobbhbc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dkkqmgal.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fzmutigj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjnppoqt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3buorljrw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qndaicme.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gmxgbriy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hwkrkdni.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmrbnykc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3olbyfjrj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rpgitycz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3amtxgyng.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwcrkkrs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wgilabsb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qsgfbncs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mmlwegqy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nsapldnl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gnutlcgk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qkarcvpu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fdvjdfos.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3svlglgux.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mffprdef.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3upeasbqd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vfepwzro.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlzkbgqh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3buotzqwo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zqtlkvai.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ucwrntwk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lhlavuub.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3elqmzxtl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cjevbogb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbzzkhqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxvlhyxj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rozfkaof.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ptdvpzvj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxwfxqyw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okcodarq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hbqpvwzj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zfeqbskb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bwidyafj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3scapuwbc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3oivntlpv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3embrddan.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cackhlmh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ujwfemdv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3eywwwqce.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tudeiguf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kgcmhyec.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lllnhucp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3pszcwypq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ahqvewud.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gfcuxsnn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tygmbese.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3llfuhpgz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rrgfojzd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xuxqxpgj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3urbqdysx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qinazkxw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uvjimfmt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wsolibtx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vuaxxmkk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3drcsuwrk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dniknvjw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lojyfmay.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3aisrdgop.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3llncyhnd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cvzmoabw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fmgratcp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vkllqaky.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rhinyfae.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3egfjskkg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bncuvyix.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jhhyeogm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3swzjlgbe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tmmpcazx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3uhpsarjf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tsdvymbd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3agzqbjrl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iwomlidj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pyhdzlpc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3phgenvxg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjlysqjw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dthuxsgb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bgiaewnk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ocmeeosl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vphqdtmb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xovhrkpt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qsaiqhkb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nigtffoj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zphjwacl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hdoswawg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xktoamad.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ilteqtwc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fyisdaur.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tvuzighj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ndvpisqh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rphoqhne.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvkxqnjy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3smytohxf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ontlxkqv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ulkqhhaa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jqjdcqrg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qpirnudk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xvzgibpy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wnqupuzj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ltwpreke.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rdyxesxe.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3oidsprfl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rzawbchx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zhcyofnl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jfvoveiq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ylrzncpm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yojrdwql.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dmfravhg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3uythqlyk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dyvzjlqp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mkdsegjx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jfwoyxnu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hvebjoxd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3spfisqdf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zxuvlbko.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3oyxaalqi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3deednntc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlpxlbhy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jhkkzazp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppxadiwz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3svisyfyr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jirelnrn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ahwsltje.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ysidrysa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yfuuhrmc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bathbzsy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wgxvksnz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dgmmdsbc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gwcmciuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osbmrulr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dhxprqhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlgkegky.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kalwpnpi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rfrdsifk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3llplyeub.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3izatxqfb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3avpiuhqa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nwqfvqis.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kkjgmotq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bvmnkvms.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zyubqner.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3prmfsvvc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvumbgi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wkgzmfjh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yofdcgak.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bowblwoy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qbspyvxq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zlxvoniz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3riakozti.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sviphslv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vcaavzyv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3auvtkssc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dvraqzyv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ogynytax.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nipxqgte.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xhgwcccn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wglngiib.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3whdoodbd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xvsrbqce.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rxdflvxf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tzvcapxm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kvyezuhu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hemcnruo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3apgwtqcc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mylpigao.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fruvhbnp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mvglnoss.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tgpbkpze.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ikqhgukq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3aczwspjm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hibihzcx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ulchfkfj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nrsvssgp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3azxtcabo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ephicfhr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hhtdpoyb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gzzoqnuj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yqbdoiow.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vmsysmwb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3adepzwqj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pgyrwymw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lwsdmsjc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pqbjnjus.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gxmsduox.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ijfdieez.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qwjejvzk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yzadseit.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3izceqwsw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vknergrs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3udobawbf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mtweggkh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3igsnfppx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bsntnqgy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3yszqghzb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wpnccpzk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qxaofaxb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rtftlqyf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3clyoimqe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cqjqhsaa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bjmzizmg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3beiljlmh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zaxtbwps.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gfujhljk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ugwyfmoq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ycxddcgn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qewvmtoa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hmfvbrag.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffihveym.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3avaejpmk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yhbezijp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hmenbtqn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qoyjhaox.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3klwoauws.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wbyetddw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bizltfno.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uwdhakcn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3oelfrzbb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ywsdldtd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3iqxdilnq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3apakilec.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ahieejma.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wfeahqvo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tkkkjqnr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hyqixxyl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ewbppnsx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rymyyrbu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lmuajdec.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3atwzmdre.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uguxajcx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nhhthgmz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hpcafakj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrewsjlr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cotsmdok.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3munszern.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rexxkona.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3thccjtod.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fdmtxszb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zwayihrk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3drhvbumn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bxvlizcu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dyzotwgg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kfeppwbw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3woxwkzrm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3otfenmpf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ucdzcmza.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ymxkaxal.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bcvszftn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xlpaonld.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mlddsopi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ycogjytk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvmcpyn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jcxvbjtx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gvqmaphq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3awdqscyd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hkzolsdb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pcumohvm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3cjlrimmd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ioxfmtnp.html


<!-- 参考信息 -->