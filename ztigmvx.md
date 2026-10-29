代发 wailian999

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gaxcduthw.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gfxnfwmpz.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gdwpfdlrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gjrpqldao.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/grfuxbsmu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/glhgtnbav.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/ghyntcvnl.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gyrjgeyfi.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gpyhjvbjh.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gebyjkrub.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/ghyriljul.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gxfwciktv.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gilqwygqy.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gaegzsdcv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gluwkbqhe.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gvqzruyvh.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/ghukewzpf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/givbhzkme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gsichgxma.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gxpqzdibw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gpppitoge.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtcyjctha.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gyikpcbrk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gmybgeyrp.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gofkbvafe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/ggutcdrmw.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gimrrrdaq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/ggcsycwxl.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/goihwsxdj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gansbpgsf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gfobtvyeg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gxptycemm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gzcallbyl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/goupinzbn.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gokrtaxiw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkpihvddg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/ggfscxbhh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtaairxtu.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ggvspudja.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwmmrcdpn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ghkpmmrdp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdbrtwnfo.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gkvmwvzdh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gvfwwqhad.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/ghmcehoro.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gconfzcqq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gtpremycn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gwpwercyw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gfbawjllu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/galsaaqdl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gaebrmoan.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gjrcdgaaq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gifofnxot.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gjocgdojr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gkhmfqvny.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghnboidlv.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gxsbsglhu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxqqjlsry.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gvpfaaion.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gviadjqjr.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gpdfolnwu.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gzzmmounu.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/ginhcxvbd.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gwqaodshy.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gbesbadft.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gthdtrmju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gnjwxqekv.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gzcdwrvdt.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gonscearw.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gvgtoxwvh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ghawxprlb.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gqjiakyww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gproddcqo.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gbmgvxfre.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gtdszyqob.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gayyglefm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gikwkafiv.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/ghsnbjppr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggijzowfw.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/glbqumjqh.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gtasmtmqi.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gmorvedax.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghqdmpjtk.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gdeprcihu.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/ghohhiuhk.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/glokwzxyt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gluhtgyjj.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/grmwixrji.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gslebsqyg.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gkkopxltc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gsfpxqpop.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gkgmjyfaf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gdbbkeepo.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/glwzmsvwj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gygewrqfn.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gdbqolknd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gkagazdwm.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gqqfgaccx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gdhltjnll.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gvdcjnlwk.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/glqaiilnt.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gmhhyzbkx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gthsdwhzm.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/goyqcpmyi.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gourougch.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gbctdblkd.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gbzpdihux.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gfamyfbak.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gzhlqkrma.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gevemjrtv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gywnqtazk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gqctxwtfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gmkxhgfcz.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gcwbviuof.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gsmjlpcyl.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gcysqwdet.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gyptmlbdu.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gojtrutae.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gnrfstwjd.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/giheiwrca.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gilienqxw.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gbuyvgwch.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gkbeoupkl.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gsdfncoqx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/ghhljcxlo.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/geovswcfl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqutfuhrg.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gzeswgvhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gtkarkapw.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gnirgsgsp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gorzrepoq.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/ganhxppfy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gccxyqekp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gwsdkzraz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gfkoivstj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/ghdjmctau.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gzmwpylks.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gvpobjaee.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gltljkuwb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/guztpnnnw.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gwmqqandx.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gccqqdoic.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/godulyzlp.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gcgduaolz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/ghltblqnv.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gjqbonfjn.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gvjpcswiq.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gcdvhqadx.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gcdlehxdu.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gqreyqcwz.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gbonnslpj.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gzwduqqwb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gwgfbmnuw.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gkutvtfef.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gdwzwoltk.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/ghcphthce.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gmfzvwqrm.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/glwgovuqu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ghzbcxcic.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gqahfoibj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gynsbhioh.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gseuzfgxq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/godnbjofo.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gqkbeymox.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gtmdmlykm.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gwslifzui.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpmjwyerp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gcvfmumfk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gakpgzxsw.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/grfquwnze.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gsrgwurhi.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gtutgktnx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/ggfggfbon.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gdigtxzbl.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/grnycmuyl.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gyhjxjwse.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gyveqnfzb.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gqdctbhfb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gcxfyomfk.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gfvgitpnr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gtytbxrof.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gvohxbwyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gpovjtgdt.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gibgkddki.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gbkqmmboh.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gtgcnjlka.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gzrylbfhz.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/glrkwypqe.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gmoxzcveh.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gjpiwphuj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gjueptacg.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gyilfzrhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gvpnrepro.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gfehhlaet.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gsdyrfpqz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gtwmvygxf.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gyndhnlwv.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gdfbygaph.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gtrukfyjx.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gjfyculja.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gqvgjpyfg.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/giutfnbbe.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gtkvjdinx.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gfmchlivo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gcjvzrojr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/ghmfvppoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gevrbytjm.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/geocngyha.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gnxrphfvt.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gnqcioann.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gwspdsher.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gzhicxkiu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gjhpyzzbu.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gjrjkfqaf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gancptaku.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gdzlhzhxv.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gkjodsokx.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/glnpqdixr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gsvjuyfdr.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gumpbwqbz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/grfzjnfcx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gwbqqykyj.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gzvhxleoz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfynnleck.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gcawzkiim.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmzfctlhd.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gudgacqwt.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gzgsdewbr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gwyisiect.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gkgdujdly.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gtblxqmdh.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gxvcsocdq.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/ghbgtcxcy.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gojtltxgv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/geprsjrqj.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gfggocrzl.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gheifblnp.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtnmcmvud.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gsffsuujl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gdwvxqvpa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gulkqxftx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gqwgrzuoq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gkiksmnlc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gyiyszlzw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gkttngdsq.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gyjnelonv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gbuljpojb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfmjfjtrf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gtjfuuqfo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gmftvvupz.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxcibdqwi.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gumgiamvy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gvdsaisif.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gbzzouvkb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gyqzfbcor.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gdvjrgrdz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gikvvygts.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/ghojlvtun.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gtlezjvmb.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gyfbbprru.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/glutxstch.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gqrguzcue.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gqaradmxr.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpksxhtwh.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gjonshkky.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gienkxrfb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gzaknahcb.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gvkhxeuft.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gbvnegbuv.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gjiewbkbz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gdsxjmtiz.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gukunkbkn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gpuignxxo.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gqtdlrqcu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gejrtixhn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gvubhvzjy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/ghdwuwqgz.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gbqevjjhm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkncnjz.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gkbwurots.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gjtlbjves.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gpccdvfhy.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gydkzbesa.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gnegzkzhw.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gkbzrsjca.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gugaucvvm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gdqakyoxs.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gsaivfvym.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/ghrypfnxq.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gvazontvj.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/grdcvhgjx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guyxzzzhy.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/giwlkmuno.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gdkligfmo.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/ghtldtusu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gykiaxmol.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gvyqixtuz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gsyxdxyxq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/glwvdfzhf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gyiqmlgpa.sHtML


<!-- 参考信息 -->