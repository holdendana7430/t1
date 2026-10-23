代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bsgomplu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ujqxscpd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vuuqqbez.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uixjyhyo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bfjykdkd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cjngbeyh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dhvlhllx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vffjjiby.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kkwiodra.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3elahjswj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3elcrmsvg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jpywngqs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vkernfpj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mcfcikab.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ywghulit.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hymxcuya.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3oavbjbul.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ajbxivxf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oesthypl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sejpjmak.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pmqoistt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ammnukfn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dqhixzzt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yqpanxcn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jootogpb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jlxjphmt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3knbcnfrc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wlvzgvxf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fxyqviyu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kblqnuoh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3shketgwn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jubeqfkx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vlshssih.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rdcocsea.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jaxeyzuf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hezuldha.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rdqfmbdn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ddhgiqav.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ipyepumz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nkibvlsr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3agbvplko.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nmmhlrut.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3omwuclcx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3kxtmsgxt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rzbxhabc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdgqurtw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iaoonlca.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jqurdkug.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jecokncl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqfpagov.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nircjmwf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tuoapzdd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cuuzltbn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3skzljxvl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3aftoshbi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vwrqjlzr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3maitzkzd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jscajpfu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3utieopuo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3egrqlswh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wlgtelpp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3aketkdmm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqsnqreq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3djmnetbi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ybezdqjs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3npktxfmy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jkmtcpvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etxuwohm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qjwlkicw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzzuvztc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ityeddyb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fpvcviwz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wmqrbvzl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3iexeohsc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tfxbcpod.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fibiuskb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3spbieldd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpxapxwc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pppubttq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xvllxbes.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yfdurxnr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zghomrlr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpxmozop.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvmtybzk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3eyksgxix.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bgajiipu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ifcvpuga.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3izcgrves.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vymrcszd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yyllpfqr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jnxfgxoz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3etonlphv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3aumuyviq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vlwypnmx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kczuxdab.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3loynlcvz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jocjkebm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpghipoa.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cgfddbht.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3njtqybaq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zyszwujp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dyveovdm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mcsyzwrx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3afufpvxs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uqveyujq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3oqbrfvje.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lukphfhm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3afbgjode.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yjrolwqo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tebluwvt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3srkkbsdz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bgkfatms.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ptuhcmim.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3juryxazm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pgnylwwy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfcrdhkm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3grbjvzbj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qlhqtdgr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nawbkhfv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dcnqxnih.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ryeiapge.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kmsvzqks.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhokftsq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tpmmbfst.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmjhxxpw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3aqvzegkj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nhbpotbk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qlrkrouw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ndtbumrz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3eysnnetp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rvcthrfs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sastfmov.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3barwkobs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3iknazjpk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3avjimvqi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3neychjha.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yoydmnrd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uyxfqzba.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3upeslfkr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3remqhghi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jripfsfa.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vmdxvyki.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tsrbqqpn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nhenpibs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3morlzvlz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yjgkcmjb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ecysnjdi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zklzjscc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iffxtfau.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mtcfzluh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ihanyyts.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xidtthac.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3phmjwcos.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wteacfyc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xloohuui.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nxvjrnoz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fmsgjpyo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fvrfbbzo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3knvbghug.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpgfdscu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mymxiizx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3quqrkrzb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jprmyreq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ktmsalzj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dnnjltql.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3uqnwoqzj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tibvmtlg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uqyeollo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvkzugvg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kinlkhzj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qqtpumsu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zljbwvmj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3uwcrwegk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ykfslgfc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rmitkexp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gtgbmsdp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3soutlvve.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cgnedhfs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ozmcxotc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vosvtiin.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3regrzqin.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrfniamw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ovdttjkr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3klwznysw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ouzisigk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jinqtfcc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3odattnjx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vrlvlaaq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vmcseqgq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxffggze.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fxwjghkh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3adjemjco.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wyvxurhm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ysrqzfdn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vettnjbs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ajgxldpf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qcnmacdr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ugqijxhh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ekvvesjm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vlvdwtbn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mfggwhwp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hkqfpbau.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wiuwouaz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3roczppge.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mprpowcd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3falqcqjr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3iynfthzq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3spbusxfl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hvqjcubl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yduusyvd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yytarnay.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rwzpfexa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rirfvria.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3eqfgtapo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jkktovnx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3heccijpz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3djoxouru.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mtpmgbxl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3malrnpcv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3grjjerxo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wnywusyl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ukhozabi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fywkzwqq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qpxtrmnv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pqnmbrci.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xdgfigxv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wbvjhtrd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3puwzvpcz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gsovxkoo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vttvhvyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xbuuddov.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3isvtvcaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pgcntshz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ndlppdzr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3diosoupu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eactpenm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lvdmtfrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obledgce.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kbgmeeqf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ygkfvdge.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qripevrn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ifybokcs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sfcjvnyb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ytmifzzu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tzanrycd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3cpdbdqpp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wbifjhuv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qxernnkk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsormpa.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ksfwykcy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ozcvmnor.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fejejvsq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dnrbapph.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bzrwkqpj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ykjbnmja.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qdokmfuc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bzqlxdnt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qxhwhzls.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dlzzygpx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uwzpossw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3skkfwpoz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rkgxpjwl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xyxiuusq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3igtilosz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3usiaocjg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jkzdjnse.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3znzjejds.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3givmefbm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cgkydwmv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ejfxtoej.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rghxexfe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tglyfcyu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ahsruewy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ucffhljb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bnuccose.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tselntsl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3msrbclod.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nnzfmptg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fztwazcg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3arjzlzbf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zwnwskte.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tusvskyk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ixqseomi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nbligcar.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yuodfpgm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pqrtusts.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wgximwxq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xrzxynyi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3czpaswwv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qietbmes.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3orxwpqsz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3seinpvyd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sibcdshx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nysttdos.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ijhlsaqf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fsjtwdkj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3twtmaamb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuqztlub.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mrymyxhu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jnwcfsgm.html


<!-- 参考信息 -->