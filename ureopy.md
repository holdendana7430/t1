代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2iwfszfbc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yvyifkdy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cnlhmwwm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vyxteuus.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2olmpmlfw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qcgjjtqc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ydvdvqof.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2sbpxpxek.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uleyklyv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2krtewkip.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trrvbxdb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wyrxvblx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wtqwiwjo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yilxepdh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ucgyagyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opcfcnve.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ihntjcvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mabqbwep.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ljjykvke.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bxsnfkef.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uiavpirm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ydlqgjqh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ywldpovb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdddcztl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hiarszzc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2alirmyaa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nqfoldvt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2epczzhob.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2udvrfxxb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2foalxjzd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2eborhwhs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2grutnwjf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dvxsfobf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2auzemwpk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qdcithfb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xpqupjhy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2supowkby.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fpshxpzf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xasurlau.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vnowtqjx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ojalzfjr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sutouxcs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iehtfaut.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ljomcabq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rhieqttc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwyfqwro.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ckvcfims.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mceovriy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cbrrltmy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bpjzqrxg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2esrmzhan.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycxpwarn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nsqqbrnr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zonitarv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lewkxfbz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cqfvvusi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ecyisyki.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2uxzjesbu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pgxxcoxp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xtktxycj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wnkqdzsq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ianqkesa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lrhoyveg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tkflvwqe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pspqwgdz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2khvrqqsb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ohxasoif.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2blgirute.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pccltpqx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fuammdlo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hhlbblxc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uupdsavh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lgwtijqs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2otvjpmqk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bgjsnnaz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tmrbaifu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uqgmnbvp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ezxzcnxb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ydgrltox.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pzcgacjh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pinblenq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hyyvjjqy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pitrgqdy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lsaomiih.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlxvpsrq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dprwplct.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sxoxhdzg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qdikfaut.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2yrdffnht.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kzqcbfbz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sqqqbxph.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2trujympd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2humrszig.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2axaywohi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ukjzbxot.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ckmzvkaw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlatskzx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cgvqlvlo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hlbyeull.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mgihyfsq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ryqilhmw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bctbypxo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2cnsgehtf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qmmpgzgn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pkslqafb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tvgubiwd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dvpipiua.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fdatevoy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ezoyibol.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2npxhocms.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rvvzbloi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zoshhqsd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2atnhneol.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ghptvkgg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nnoqiigr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pryklele.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrlatjpi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2thpbricd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zqvoizhq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kwpgnovf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bzkvkpvo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gkmfhdgi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jkenswjl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lfvpcykc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wrztlofi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wnphfuqd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yyoxeynh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mawybcdn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wvmbwrba.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kunvbttg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fvvelfqo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cqcmrswm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vayauxwa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ziukyxxp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xncdkgpg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wmfozopf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oquscghm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2aivpjhof.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2gskuodnf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zwlmaoso.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ggsndxvn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ifuxaogy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2sdeykeaz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2niwvvtuv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fvukvjyx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kietmmgk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gebsmmkw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2syjdqhxk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2eypcfgmm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xusscbjj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mlashkpa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hsxznnps.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2inolleff.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yeenjixi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zctejvoj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2oxwqikrh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pcvngvov.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kfpyfyum.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ythbhhpl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2iqxunhrx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wmnxxhmh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tvgidzri.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ijsypzvu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2onhjzhsz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2egnzxwoq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wxtikdpn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2elycxudm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ylazmipd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gotvoitr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xnabqeoc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xfarxfkn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhhqbnuv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2woddhcjn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2skowrdmm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xbbbygfl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2abgxbmrf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fwfjohli.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wxnbwzvv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zesxfueu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fomjoqht.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2loiqamjo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2slnffzfd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2swrkchyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaqzagvz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nejeixyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhrlmenb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iacuessj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ckxbrinf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbehccja.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2udjxzstp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fivanwiy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2uxnzfoxb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yiixrpfq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bmjijxeq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fcyimvzo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hofdkxax.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ifwgkwzx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2axhkaojj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gnyeunld.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ufdsahzs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gaxordsf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ozyenhar.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rxteqwpe.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2nlaquxso.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lrbfgolh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cqthtgwv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nnbclcjj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbxzyesj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ciiwocnc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mwgtpqfi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ntpitvwv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pepwwkwf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tclgqgwj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ebireumw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bxgtrtuo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2omdekcez.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2punwvudx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bovqhoix.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vgjxtseq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hjuxkxur.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ykoqwtep.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pahntwlr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bhqacoed.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xvpekrzt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ecaeyygv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ibtxabzy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oobkymgc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2azijkyhf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xbywzfxa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bvcympkp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kgtdqnrx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zvgqapon.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2camdnshe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yuyjsarn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tsqtwxbu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2enbmptrq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qqjyuslm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uensuahf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fylimznl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mpsbsfqv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vhvpuzjz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2oghfeeld.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bmnzckze.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eeegtupw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2acbkbjzo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxpclmlj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2muplnbts.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hndnzimg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2njmtadmq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2efustzfm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jespdjws.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pwmzzsgm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2izuuzgob.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2exumpkxm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nitntizu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2azgofeif.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sifsvnrq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2chnazsjd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bvtpuopl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2sanltlex.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hnifvigt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrzncamg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2mfnabqnn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vkkotlny.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2goywwqkc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cvumfscu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tzcrobss.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zdghqarn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gaidcaao.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2prumgeys.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2eqaqmuiu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ihlbglgx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qlzpvnze.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fwwokgmy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfesscqo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mfxpnuac.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ckdbzeuh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2irtwchnq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fjcaatwm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwgmwonl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ultsjoex.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lhzppnzb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2heuiknae.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rtmrngvg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pvlgjhfx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sbawusgs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtljgkfl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qdeihnkh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sysncxde.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oukwgzov.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2feclhbhp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vqixrimj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rrxxcgyc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2delxwxpb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mecizfqu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yikblsaa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrbjuojm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2enkspjjr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lguhfqnu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cosxsfhg.html


<!-- 参考信息 -->