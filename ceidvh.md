代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3uecqgwrh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3bdunigro.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xoomrctk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zxzuoyba.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sijedeub.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3aeonjapo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nzorveae.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3moqueuxo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wyhjlnyp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sgslcdqz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eawdsqis.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3snxgovcj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wuomotvl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jhzcwgjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iuiprzch.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3cwbsjclf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3knhjyexr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zwktykob.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kkkpkswr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3evfalcdj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rjsidjqe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pvaawwsk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nwzfjdtb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3outmkztq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3eacsfedf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ivrnrzqd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xlzjsgzl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fjfizwoo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tnpsiunw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vktdynin.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mwlnttoh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3fvxlomsq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fprubrzh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pgfsssex.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lbkhsexl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gtuozdbg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yzbqisqn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hwboqmso.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3egudebkm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lwmuijyn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yyvtankf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qwlegigc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3uqqnzwfo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tbieyfui.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3afagyitf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lgwmdigq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hepfltoi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gexsfwmt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qktoljmd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lystxgeh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rlhxlyvd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hamjabrw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3swvjrgeb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3sblytflk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fojjeegz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qosnlvly.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qrzcigiz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xghllwig.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3udzvckmp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hecbasat.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jmzhhipf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dadphhms.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zjtqnqku.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edkpyzhu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzvnwyue.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grfeutmq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ptbqrmfp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hqzeoced.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zlallvdt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tjpdbofr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3obecbycj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cujyqdgk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qilxlhyb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yvumpdix.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3oafhofka.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wxlideqi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sqcsqffh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jlzutoej.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xvgjutnx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gdyvsfks.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qqouakan.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vxhsxntz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yznsrsud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivraalvn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qnfxkdfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abivizds.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3grillvqp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3drnwnngl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yzdcaanx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wflaricw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xxxbnybe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ziwdomjv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vmvnlemz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ncubwvhw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ajixufnv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pcrggkyp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3esztqfsl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dyqmkilo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghhmbqjk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ycetdxig.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vvyngjrp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lbkdqhth.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qxbrddsu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3woedqgyg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bjsjptyk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jrmthaty.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cwxeuliv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xheneklk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3aequazbl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zkcitpje.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pexcdfya.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nicqcjtx.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vluihlia.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3pktnscgs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzlrnyrb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zbathlyp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sorkzazl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hehjuqjp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xnzuhpug.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xrvemjwq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xqllbrdg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xfdnuzpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3inhbavkc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3syqxjdmx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yclosxkz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3sylpjoid.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3odhxqirt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhlauzzn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zqtnlhgm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3udmvginf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cntjlbjc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fttdzsmo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jsqxxgww.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mnlylswt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3loswjyge.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tcsjxvfz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xlxlzvzc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rsjoccsp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vtlkypjs.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3plawdohv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3osyhdgji.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pkxqdsqm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wkaqzxem.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rmzxkpfz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lnktmwxv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wwpmymmb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xydfyjtd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ywtzsrwy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rjiatrkx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jaqmhkzi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3sjdcyzdb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hcleizux.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enjnxdtj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fckhrpuk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yddhmyxw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jdvmslim.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fhheujoy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3awyrejms.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xvdobbon.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3twzlvvay.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dftxpslp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rvhbeywi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lwatbouh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fgihvmrg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcqrknkg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kmsgphoa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kieyheyk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jhvawmjb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ybkwewqi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3blorzfqh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ebwojzab.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qrobvveg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3szlzmjrr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wwfvsvxf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ismxyqgs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3frqaotdo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3etcbktpw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fsdfvpfu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tgctwxku.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3znpssnxo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nlxhenhb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hyzxgdbs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bptppagq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3glzelizk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nmkexhki.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dcgjdelt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kknaqxft.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kffybjwq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bckmvruk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ukemzvro.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kuauhprw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iofwtvvc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3lykishfl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zgskuugi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ynnepclg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qnuvbbvq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hgeaeyab.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qsadcdrv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3suhvimci.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jgcfbqeb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vyvjhpik.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3akzohtpp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dzwxosxk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3msvzvtgj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ddmaihxk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xsavdjpq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nbpgfjrb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ubkbugll.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zppackns.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vrfhlzkd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3lvbknicp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qbmkvvxz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fcajsten.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3puffynba.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jkojuzct.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bwgxyuhe.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3flrbepsf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vxfzfrqa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kpalaomu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bxgllmhc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zvoxepwz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hgiflgev.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cddlauiv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uaexvfdl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lzagoszh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zemjyikb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gemobxpr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ryrflwas.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3tbhwtoqq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wjvrslum.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wgotnsqc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3azrltuez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dguhtvcl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3noypldzt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3llxuquhi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uazaidav.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pnselsre.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uxinxjwe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jqhznqql.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3szeegenx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wsaxxvjs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwanqpzs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yvtkxksd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dswmvwgu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hsyurkxm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3febuaqlq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xrlcovzc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qqliudkc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3habbzuho.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3utaqcnru.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3txaxfabe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3meljwjkb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qcxrlfor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odiwvefi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yfitrkae.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gzjmdezc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zmrkbdyw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3eoecjiwc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cancbbij.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ghtsrruf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cuqpmkel.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3efpqetbr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3orgukufa.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ipcueakh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhygpjjd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pqzxzmyj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3icwtllny.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3uqstkxfu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zbfhxvvv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ccqsrsof.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wdgxtxgu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wlhweuvr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3apdudpya.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xohkiksx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ekciwmaf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jommvlzw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uxbewjig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdwtfxe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aarlorpb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fljhehcw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nfpoavyo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hiyqouyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nsrcczmi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3idhoewyt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hpjefbgp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3angkcjix.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jagcmbei.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vhkzbuan.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hiqngqyr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tjzzebiy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mmufrern.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3djdynmpr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ptckmost.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ukinxzvh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3judqxasi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lwpsugnw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hrjbfgcw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3igcsyacc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ebcccnsm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dddrlcuf.html


<!-- 参考信息 -->