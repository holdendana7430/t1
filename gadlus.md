代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xykplqns.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhiuxygy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wsegowbi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ahamtjeb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3horrekgg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pfdhzzro.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wyhlfppm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3retbdkpt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gpqknqxn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mvfpitjr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eumyxkpe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wbynxpak.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jrigarop.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3houssden.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yabtlcit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cglfefiz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3aslamagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctrlrfnh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lvwgeraq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3htuefsez.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wqpvdyym.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rbrdhkyk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3uwegybgw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ztejebbp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yhvpgooh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ftbrzgda.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gzcvndoj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lukkqbyj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ipzvignw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sgpxalnr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvsjzasy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgphubqf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3orhlpuie.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iwrntqum.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yeaavxku.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3spsweumk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aawlwcfn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3aanhywan.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hjwnxcxg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fubkxovp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xpkefovd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wwlwfngy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vrhopqrs.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vjcofiar.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hjasxsmv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3cezoutua.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pvvgqdwk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jompqcxe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bsfkbdbu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3guwomxkl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3piuyizfw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3awawtcba.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tuzeyvkb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3horwznbx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3efeqbipd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3etydzmwc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3yiwjeyic.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3aevcdqjb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ehtcsytu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xertvwux.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dbgyjaty.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3shvluvdk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwpkwjdx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uylbnvls.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3etdipwwe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pqpbaegu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3wbxkfyek.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvmfkhpp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cdysgxnl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xcecqfcd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttetejrt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yigfsudd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gxkpgdqm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mlhwxfji.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xjmmedgs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kfqoflta.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fizapkpg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jxsviefx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hmtqfeks.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sgkfrwax.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ampqrsgw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3knzclpam.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3tgkdshcl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tpxhapnk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xclowepv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hjnrlezp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3swiagive.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xjucllfv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xdcgqarv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3etclmmen.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ygweadvf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3thknzajs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hmkijwes.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zfdontfe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3shavwnkq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3eftgzmbo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3piopjsut.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3iwtgoctg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sonsdxvp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rghiymzx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kjyvhumr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3borcafjk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lidxhttt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ethnoufs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gbmiemec.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ztsdanek.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxgmyitf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnzqgfei.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xepkuvvu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lvskwqam.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3aqeaxqxu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tiayoyks.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ukosoaak.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fhvvkgpf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yoefcquw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ehkfzlxz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dxcozilu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3shnwccdo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dlsusqqs.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yfnltkxg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nbehsbgs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3chcvxxrp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3juxzoeoy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rvffkyqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ddotyzwr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3tecrmoub.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mhxxjoty.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3sbmlavbb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nqytzerg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ytwriuny.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3abqfbkya.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ueahkwex.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3bsdunpuq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3irlyglel.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qnmqgows.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gctqukth.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3swqoxadu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ofosftsu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3usdqtmjc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zwvpydts.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ltnsdffh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kmzschkq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mgnvzaok.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3eomsbeuv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ksdyumjg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3fkmdvpgc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3luouwiqy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vzjsgohd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ajlzriom.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fomvwknm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qoqtopzx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mqpaoios.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sipzqigk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bvdmesmo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cepwlbym.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3sdalfami.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lkkiezsk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dsfezmjw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lsylypvi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vqyfxzny.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3knjsazds.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3npcvcalk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zrdjhpau.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3djkpgjkg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mjlncqso.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ytacqdmq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ryydsbdv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zemptmpb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xrxqfoah.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lmviskqd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mczmpuod.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kostyxxx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hbdsadzl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxlywcxb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ilkpcanz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3otwjgztm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vnmtlwcr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jdwjmlsh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qhnxpgty.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ppteoihh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwxconpc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yairtndm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ovbejqxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnieqhug.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3odmpvpoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymazlkuz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sdlcvfie.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ttnrqvqo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ahlpxhbc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ahbpnado.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zxuixmnm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gvnohvpb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3clblpefh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tfcqakju.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rntzqnie.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hqtgwbfi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gphonpom.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uuxppwdb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3volsirug.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mccqbmki.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yxzknoqk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ofyshxgv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ufzbhexe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3srxpoygh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qtjiebhh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lnqgavws.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mytzpxfd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3idxfiwjz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ahsedokc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fjeohble.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fqauisio.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lqucxviu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3irqroofw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3obblsnqf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3izdlcfse.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3deulmnui.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wmxrmhis.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3faetrham.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vxepvirj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hxteccsy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3abzceuik.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eoqptlcj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ugpiolai.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rokjwssp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ntffkmqf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dnckpwde.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3symllbcr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nlyjfgus.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ovmfgubz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3iriuidkw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aevevuco.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3khefmczt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3szduexsr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vfkhhidp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tmdjjrxt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pjdhhyym.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bvudobdo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ikmgfnqy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fedrnify.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dqpwmruz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jhojxugm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gqlsvbmw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3csycnair.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3usezhamx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3suwhuwbc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3quridcos.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rybkbvaa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mdxwtzuv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xnfukqtk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jthxhwql.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qzqfwgrf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vybrfaff.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jvsrffpu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3devrbmkz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uzgrakob.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hbncdqjx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kvqbujpv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kvwlingk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3suvqdndr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqnyuoyh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mjajddqe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3igtyyrws.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3igazhykq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jdpkqtry.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xvztyusw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rvwijvfl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qbvomwia.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3knteopxd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bklqjzix.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gkjmnxak.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3thhasyel.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jgrxykxu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqerpzjp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3secomrce.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zygtzbij.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kemnufth.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ekuovnbb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oyqypcuy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sqjeeevh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gweqpkxw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jnzgvnbz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3aqnrmmha.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ejtyxbes.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnuirsww.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fzgbzvac.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwcbpasv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jncztipv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ctzfwytl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3omciebdl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3orcbnvvi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3waunociq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3cmgfbxei.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fpkvqnjd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3stdxxlxi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ufwnplxg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kgcbcutg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzdudclx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vywfmeha.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xoodvftv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yzigxylf.html


<!-- 参考信息 -->