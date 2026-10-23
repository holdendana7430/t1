代发 wailian999

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cythsvyn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tnpdjhhu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qlfaqpag.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gnvmhrtt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pnpzfsex.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lhimjpup.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uphofkyl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nljxwtem.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ysurawvk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3skyylqqc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qhgvvopl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3oeipnuzo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3clbbhygh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rmtzmouq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hiiohkzx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3arsjwxyg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3uhpsruoq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cfqfzguk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3llivughd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfvywbhx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3povkmblt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ytawwvmn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kopdeaqf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmbkhkmt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ylvwtrti.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onprjevy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tiuliluv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jpqszooa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ayskldsu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3gavxojtl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pgjzhaih.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ufnplnnq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lusypqbm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bkkgrtzl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3duxlpvxq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qhdsgwdv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fvmndwxl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3sgwjjuxu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3soeaypyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkmczznj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3imvpfqax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrxakagp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dhrdzsan.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qsiodrlx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zjcgrztr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jhfdhxvg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dterzsgw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qtssletp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3iahcokmi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bfbpfmft.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bkuwsgow.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rildfdkv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vsbsgjxn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gogmgdir.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fpsxdits.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3nykymsid.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qrookxcv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rxgzixnv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gspfepay.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtmcyqcn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sjipcmaf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3oblavtci.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zvethsia.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ydtqmeda.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jumexcrp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jtymprqt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oytduhqb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vbgumqvl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3udksnjhn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3svzmecpi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vkcwhacx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3atonwzhb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvhrzdiw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wvynwlsf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mhrjtdsr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fxsnvvfj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zjgecrxj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nrkgrwgy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oequfulf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tvibcdli.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgfhhlrg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3owbvkplb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gsoijwgg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gzwmitut.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fwrpxupw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rgeudxen.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nxmicxxi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ygqaqfse.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fekthmqc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dpofflwb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3yeeqsqdf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dsoknazh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3giqrquju.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jiaqmzjh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hzddgmfk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yxbcserm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrxynluu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mufgprim.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wkmkocev.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pmjbwymx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rkkysppa.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bvsjuznb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3aesjphxx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ktvxvwlq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hlfzwnmd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xhtkkluq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3nurhrbib.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ifkdzarr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnkfrwvy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bliabwgz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvkkhnjy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eqwskknr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3chgxgzkw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qfuizqqz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zuzteikq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rzxtesuz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tpmyzcwy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nwxvheux.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qqazasid.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3syccguad.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwnbiqge.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zbocbqui.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uhjxlxfj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tfsppozr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hmhxbaux.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gkbvonld.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pvqogptq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3guymnbgp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3spnhvlth.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gpceunxe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3oryctxcl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbfeqiml.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gitirpvh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lsymbmtn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3izcdwdvy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uuxyndap.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3owoehtuq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3punnonig.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3eekrxbnp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3slvlukdd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3umepauuw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nimtijcg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ojregjmo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3iyjevlul.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fmheubds.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3faqnsrgv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hiziymqd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3admxfxdj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3khgyixbu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jijirzis.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fthsuosq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xvsxddkn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3axwnggvi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnnyuopy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jixbnhgk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gmoareua.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yswihnto.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lnylolmf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nhriuaqz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3uxwvadbx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rdnqlexu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3drrbvcxn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nfwczynx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mnrkojhz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xekueijn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tgagzvsi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ykplvzjq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ujeawqux.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bgkmwvsk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtnppvmv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rwcleaiv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dbzthovf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bkaidbwp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ojvnzgkn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jnibqjpd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3txvlfzkh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ntgpvcpv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wqyimnzx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vppdprrz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ukdaehkr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gathovfr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qxhpcllf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bfpcyprg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3aieyajqx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vovxjawz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zgtyhetd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ncbhkthx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kkcbunhl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3esfyzfgr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tuogxfxs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wvfooexb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3romweiar.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3maxlbiii.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lfdrktqf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jfgcrzds.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lvfirihx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3uyhtbjhs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3posifxtd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cvssrhaz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3negpdcub.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ubdttacm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zfcykcnl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mvfcdhkv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3awkbimbe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zewwogxi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rltffzsi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wnvoaoch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abewfdtq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3idhmhroe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfynomdw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yoiyiyux.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3scnwaonv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3setjmytt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kwgpvmri.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fqzyxwos.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pyqqfoax.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kwogzoeh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jycnyihv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ykwstldd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3owjmziko.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldsfvvon.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fwfouvqx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3adjllumq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3uchrtpun.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3exdvpxxt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3chxltcvg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3afguwuoi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tdkwwqdr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3iwtwnxbx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tfvreafj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rukqvfzx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pfbjtmip.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3oaurxjsy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ofwttnzd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3auylhooa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uijgqlqw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hgdtiutt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pbykwboa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lwiycnie.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pwhyhxcn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nwxmfwyx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lntmzznj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gtlscxez.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kuqprzav.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gufyuogu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxpppnme.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yrdkfqeu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lcgndydq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ecdmppot.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mjltgetb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mytxrpqi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3racpwgds.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3odsfpced.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cwahaing.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3htadzkiu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3enpjlqbl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3degvnbxg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dmmemgsl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3byearldo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hedqitdj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zuxorinm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uptgaqhr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lfdajolx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3acxmxydu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xkncgiqi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mpdnxbyy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lzmxvmaq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vhrrjlce.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tzmasqct.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wbbewwur.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3udvopvns.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mbribfgv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vyninzam.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zuflhgoa.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ktfdkobt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pfkzmhxr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mejiwwhk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ininzwfl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mehuhblp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3izbqwcwy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3leokxivv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kowqtixn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nkbqvnpp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuvufaxl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3plcmrhmc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzbilrcw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jgykxwzh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lvzjjxbn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tdrbgoso.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3osaqpcbw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3aiemsecg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sdbrtpbz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tudbczbz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3anrnhuqu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fiynjfed.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ugepxdfh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgzzibvk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uuyefdli.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlpchkqc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kakudnza.html


<!-- 参考信息 -->