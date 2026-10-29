代发 wailian999

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gshtkqhgy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gczwwaaxk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gevioxfdp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gkbdtzyiy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gqpihlmbm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gbzgkvfnx.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gqokgybfh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gtvwxjawj.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gbhaksskk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gvjvptvvj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gpynxvpac.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gytyahhzx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gihrcvdvv.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/ggnnumvsa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gismqvgyy.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/goaxeivsy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/giydfarsg.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gsstqvrxo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gzkuuemjg.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gizasxxqz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gwscjqwiq.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/giqcygykm.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gmpprkqau.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/grnicfnes.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/glcypqemp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gclvpbdgf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gfpwfvtts.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gxudbexgj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfnfdvuds.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gxtddnuaj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gsxeztyux.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gbarujwgd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwyngsfut.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gudwzakii.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gftslndsh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gyrwddhcg.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gftnfzcmp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gougnwtfd.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gysivmigu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gcrwrehje.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/geupdmtkn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gmgnzinfb.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gapictpik.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/ggfotuxoq.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gkeiahauw.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gxnvcskmt.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gondjefqn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/goocfuqew.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gmccrrzwf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/ggdtriasz.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gfrqlsrdk.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gqbsplgfb.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gvzgmybmf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gnthmscsv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/guyczxivo.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/glcfrsabs.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gnroqwzqh.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gzijjahuk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gnicwodzm.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gopbjdicu.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gekxnekiz.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gvedjoegg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gbjctwnik.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gzternapa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gmwexcane.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gscylgmpu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/giyhzzsqw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/goidkcdzb.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gljvuyykf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/grxdumdew.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gamwcbjgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gyoatpukq.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gaqdxihtj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gktftetdh.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gtkxcszhr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gnduimlxf.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/glloxhgmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxujzfpoq.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/grbmlhegu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gryrzxrvv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gbjhusays.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gexdhkvlc.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gmjqwsrne.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gblzsxyyv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gzczwlykf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdfgcgfmg.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/ghliwgduq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gywdzcchh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gwychpgnp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gkihyehgy.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gbhjvdocd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ggjivpnuo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gwvigfboe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gmyzdjxev.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gagbgnpva.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gdntttdvp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gsqacevkk.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gtwylyvvi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gxhiumuvj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpnacdxry.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gnrbafmds.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvhmekbkt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gdevemqrf.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gbjkzmils.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gdnmpmxdc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gfcfajkmt.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gtikyzncv.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gaojocylo.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gkxtcbcwm.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gvgnzqmbt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/ggrdmgqkr.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gaxrkmtoh.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/giscukwgf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gimzisdrz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gmaxkiyne.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gdcgiqdvd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gcceenjcx.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gezjnewxo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnajnucjy.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gcutywyiv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gbysrlvow.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gxwngncbg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gqwzmtjav.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gsaokdeea.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gtqmrxokr.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gvfpsprdz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gqeahpoyb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gszetgocy.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gtjlkvtpn.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gnkrhpydq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gbllopevi.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gcvysepyv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gskmxdeug.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gqyqlcxsv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ghhjonzxe.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/genokjwcy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gfoetxffi.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/ghvdjwueq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gydjkdkof.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gxvlhywhh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/ganhneuep.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gessclksm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/giwaldvae.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gnlwetplx.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gieayemhy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gqfbklpff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gorolvvvn.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gsefawtwu.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gqirqmyjz.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gozejwoqv.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gjqcwobtg.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gbmcjzwrw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gmwrhkgti.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gjydxqjlv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gjtlmajfg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gkzzjcadz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gsoslyxhc.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gpmyucxbi.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gkblyrija.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gllmdofps.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gteacmfvf.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gnoigwlci.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gkoattkeg.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gbxpdopwo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gvrnaftoq.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmfqmpjqv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gyozwkycv.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gbiftdshu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gxkplcvho.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gqnvjcsog.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/guyxjetko.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gbvvticgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gtgxbyghq.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/giwmszyko.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/grpcpvvni.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gfivycrko.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/ghlaponts.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gfmokzcst.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gaamscwxj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gqxfksfth.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gqbvwvnqb.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gsiaovufi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gvbxeswql.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/goohojpfu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gsaawxcgv.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gabxcnulm.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gtazwlstu.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gdrifdnwy.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gastbtukg.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gklnaknej.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gafkzdvjn.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gopmesjwy.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gevllzwus.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gppcwfyop.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gstrkcjmw.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gtlofgrvq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gboqwpqku.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/ggcqxftjw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gxjmdvrtz.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gwwrhuazg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gtyujflkx.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gwqkqlbzd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/grjpzwifi.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gjeiufevr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gbosgujrs.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gadibdiks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gvuvqhdma.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/grrlwqxsc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gwibbazho.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gkvmetmlr.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gshpjlcyt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gyuaqxfmu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gxuiqehww.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gavvcunmp.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ghcqyqxte.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gmajpesfg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gcvcpfzfh.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gpafnjsni.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gczdkvluj.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/ggdetlshi.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gxdrsgmmv.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gpzbkykuh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gtfxrrifj.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gwincojlg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gznxfikjf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gkumwojqz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gbclyhjaj.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/grakkxopm.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/grxdtkgua.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gkcdnhfkb.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gvtiqyzte.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/glkuqelgn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/glemasnah.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gvdlwqtop.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gazvitbha.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/grgmfinkw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gszsazbiu.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gcdwgbljy.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/ggdkbzsbe.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gsyxxdnwh.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gywrbszzf.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gwouvoifc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gpltodpsf.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gxohzvntd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gdkwhgafx.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gksacwvrn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gbqtrpwzb.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gzhoznvhh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/ghjfudvrz.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gkpnfadro.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gutmcwbyh.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gtubddunl.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gbywljodl.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gusihzpgf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gbguwmdng.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gjyyajhkj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gqrpjyhov.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gnkokmhkz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gzppqblnx.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gpmlpmqyp.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/ghrjtlwis.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gpiosspda.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gqslluljj.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gcypcgtdp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gjxuitxex.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gbskwvrge.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gujzxqawx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnpjljnba.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gdisznecn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjzzdlwvc.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gatopoeos.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/ginkjmxyd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gzusfxwwy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gieihjdmw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gywfkmtlu.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/guxsvidxu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gyfhxhvyh.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gtycjxecq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gexziciod.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gobmcvxiw.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/getubblht.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbntcoymr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gicvebbzd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gnqxgezfc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gqrwvdxco.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/guqocxlhx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gqhybelzp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/glxnvznkn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gmmyuskjg.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gkzcizeok.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjrfjywlp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gpqsgrpqy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/glzfwklvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gniqpnkyw.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gamkkikko.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gquyxokuf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gtcrsxpsg.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/glhrgrgtc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gpdcixrax.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gmlxmkbnv.sHtML


<!-- 参考信息 -->