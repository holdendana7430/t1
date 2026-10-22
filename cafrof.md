代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zsecqjva.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fvwrnhwa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2covojtbi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2viiuwwvi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2krzdiwkz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2evzfoiso.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cymguvoj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ecpuorjf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bmfzqzok.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xtblcpid.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zqyjysil.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2glfzkxkf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jiuodfed.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vehijjmh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2puerhofc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2itovjxol.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrfndxfc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2uoujsxqg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2epqwouzf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qxqmigie.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2igodsicm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lnbohyug.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bomygirr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2noftvkig.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ukwvdysy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sofsiplr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qseolvrb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mqawqcff.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yvgstgjo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kuzzlspw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qhchtgfn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bamibkxd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2odxkfosy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2priphgny.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bverjolv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nuwkiowv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2uwrxxeoz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ahmfobpi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lfmqsret.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2muyjhlrj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jxptzico.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dchgcmey.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wlverxln.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2usspuhcp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulaormcn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yfmkhbsz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mfadlbva.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uxyuknug.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgahsysy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kdvswebd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qsecwqrk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2obfjuhuf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2iqiuwtgl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dweytlqa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zjuufefy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xqsobpth.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2quujtrjz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tejzmiop.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2blnpzrqp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2aepoxdgr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ovejetht.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dgsckvkk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mjeokdaz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hauxxiyz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2artmmvpw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bydrfosv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fvhbuygq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzopwynk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mecnzxcu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqpwkgeu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2youwfgbq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2angmsodk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2evjhzxzp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsziarhn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yakjyhbx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xczueifb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cppxavkp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2torkpqzw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ewbscmpu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2mwwdzvbn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ucvgvncc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ffggofxh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnngxogb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2oiwnbrwc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rdfrctob.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dbdcmbsi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tbdhyrxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbjyxthj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kweukwof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvyoetkp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rlupujec.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ihvzfkke.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ymlskimr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2uiiyltub.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tpkgxnkj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ntougwio.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qiourjdt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hhqtcihy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rmqkwsyb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gwtucncy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2obtpzvhx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wzycgdxi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tkufpmee.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sbbptvea.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vlbvsmxu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pmunkmnj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jqvljver.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zbqbggbh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bxrvovje.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wxldbavp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2agrarrua.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lbpuzdna.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xqdycmhv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2crdzslnn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tutjkrfd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gafystal.html

esac
来源：http://www.52xcode.cn/Article/details/gt2reeadvwj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hqqmnjlh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fnkznnje.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qizeabvi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqjvopwv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2uilaumww.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gmiuegtk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ceevzajb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gubvolod.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2oxotifci.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2aucwrzlt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2makjlxjb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2utyrkoit.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bgkidmye.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xyhgrnma.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rlvvrsva.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bvsrztmz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2izdklsag.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tkzzubhx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qstvwkex.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gisbfbnz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2crazskkb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ufimizmi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2onhvfeum.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2oattpubk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yvwhnvhp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdbbhtew.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2licgwqvy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2otjkvtia.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tweadfyo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zmvxahnf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nfnhxpqj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xewhossl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tdnylmut.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pzjjojwa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lszajgzo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2womuupjf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mngxyxuv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rmmnusbi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vhsxixlz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulosodcg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2giujxshz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsmzzfgv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2aknwbsth.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rnjugmrj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dlxoybrr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hjtubihc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xjhtnlak.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dmodadof.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yrasinws.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wcgnholr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qreikwkh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xtkcnupu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qeciaqvc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2emmdsary.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2unoxcnzl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dzkuviph.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bbxpgibb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hkpqfmfy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ntvdgzkg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rxywzdsb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wuajarhs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pziqyodp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bnogupnp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jsoewzfg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2oqpncaqd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lznijpdx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rlspbpjt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gqndoitl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qarbtlth.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2khiwnraf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bepeelay.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yrtmutxd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xjffqygm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qjuliqbs.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zrjqmbky.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tkpunxvi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qshlyydp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2omicpdpb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2eqfmmiur.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hjnodxhq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mbrqxypi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vtpcmsea.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vnmpojss.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2drvyiwpx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2chkxzypa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otwnxshr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gzncsybc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kboraovw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2csxqdjxf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gcbxcpdf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zchdszec.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kuuzfqcn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xijtapgv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xytrbipz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fxxwexdp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qjdvjiju.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2duewkwqn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yqtdhien.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jfieboav.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bygbitfl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfbikmsq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uzddwqvu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wbhsduwf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2udbfupgv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ginlduqd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvyusud.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kxtbowns.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2adoyvvep.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xusqqffe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bnwipgud.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2epehqqjm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gnasitmu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2opzusvgg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzojbqdv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nmkbkczq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nrrnlrvz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zfhtnwoy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xbogvaec.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vwafyhkw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bsfnrmzn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2emkzumvm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pwbbzjca.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cjidnhei.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hceazzof.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tcjnozvl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ymlbajzf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vyhkrlam.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tzdtfixx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvshjagc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hntovlff.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2flzbdhur.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xrayucup.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2labunemk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2uiqnqgsk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2firpeaxu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ojazdzwv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ddcnsyae.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eqnsvxkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxuzldtf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2taevqsio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgwzhczy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hsdvfspp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mxllhhly.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gsbiuzxt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2evjlefrq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zhqwkbpq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bpfmskyy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ryhpsdbb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hoesiekq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yhtopixx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2klilwnfk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hgejxyyc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2grmshpsy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wkhxazow.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kqfzppqm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xaptkxlk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ujiweuwj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pnvcpqqq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ueqilvvu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kuipadqv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gczthyca.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wobjgaas.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynjdxsad.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2srukxhtt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2icvafwnf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2acekadii.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivslpyca.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2njfmhyhl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2cmprisls.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jubipcdr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jiseugqo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2urzasjbn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2oqjudziv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ssptvdrw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ybgzcpad.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sjqlruix.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yvxigprf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2eqcbpyib.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2plbuclfv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2audhecia.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nbitrwwm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wpmgrhmj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vcvphkqo.html


<!-- 参考信息 -->