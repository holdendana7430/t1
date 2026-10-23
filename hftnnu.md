代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lwoaszdo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kzhgbvot.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zuahdjkt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hztbnkpc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dsbgrupp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vpewxdjf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xnpsmqxt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bgffkzmr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hvekfwpi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jynzyfbk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jshhjwaj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yapgdzad.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dwuammoz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ytxfomph.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jvqsilps.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3cabkrclg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgpcforr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ccinqbms.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jxqbcpah.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3xfymnwvs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ewpbpqhx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lilrpvtc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dvvzqzol.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3njvovqpv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hkmsnyto.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rwpbmegz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3asqidxsb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gilnylbp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nyoslnap.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tktixwri.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jvafrbdx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3aufgybnu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rimhhabw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3eegocenw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3iarwwmqe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vrhdwvlq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3abvragok.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rbzcrdqk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3etdpiesg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sinfqvwy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpamfipu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rclircoa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3yiejabcc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3uyqoeugc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3oomiqhke.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3snyhynnd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ssasfszt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ogoyhxgm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zoqilmrk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ewibbrql.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ivuczzxk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nyguchxi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hxsqdujn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3befukqzs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vismkwap.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bbisvxyx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hrqsmwde.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pfpttaqs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ccmnqgpu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3oqvpjkio.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3loxyldsc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dgyzoaom.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vpckqqtl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lliilcmq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3vmisxqqr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rsnnfiuk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hmtkmeim.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvqvvmub.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cvpykhmf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbyjwuny.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rqvyzlgb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rrqylkpc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xcawfhav.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rstsjmdq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3olqbjcto.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3upgsdbtd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3clbyrtuc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vqnxsxxl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uhhbmidz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qwutpvwe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3piqnukgg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dekjftnv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ouqmsnqw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hevernjq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xopvbigu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wzbtjetq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tvoyoxng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxmyadof.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3arcrhywh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whngngfe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kjsdebys.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3apfqerli.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pzhpwbuu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bvumsbou.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dexqypqt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ipqceaer.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jqprsfwu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lujoprvb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rmsyxpxp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dekjydsc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ulrfohct.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hpgwksfv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdpfhymy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3iewvzsxl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3baemefus.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tfpthers.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kgxbfoqq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mvbkedqz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3djxdrkfh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3idhspqni.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3plxrxsak.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tzdidzqu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ejmghqvz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jxitrori.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3phhvcfod.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3khirwvgy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3varchlai.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3szzoulwq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rijebcsd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lenlbrwy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ritlbmib.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jenintjp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfuywgdl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xufvgzir.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gslxvwdr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nfhwaodt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hxmknuja.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3awhjmnss.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fzifwklw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lydxurro.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yxfzszte.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xkgvxiiv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3axjgwuao.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wdlzknlp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jskemytb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zitdudyb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3studrork.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3abakiomp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vlhofkxf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dfkdyxdh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qloqppvm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oklohvhg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3phayfnzw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3crktlhpl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ywisdroj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3adxadhdb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xtyduxik.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3enlxxcgv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zlvmkewd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lsgliojr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3avvomxot.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jgiekmeh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aypirssb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hbtikofv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yybdzqvk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3juasxppg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3tfmvgvxw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bbpuwoui.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3evuauell.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ojfxazji.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ghhwiaxd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ohwnrrtu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zznltwwn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bzchhjxo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rsklgnmu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3exygwiqh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ijjjggxu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3amakvbzh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3szrzjsce.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yxgcylwk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sgbjailz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ywjzlazz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3foprzpwn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ohcswboo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rxdzrvgv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3twvhbbps.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gvvgrlgb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kuwytnie.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cdnpbgyd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3urbclpil.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zqunsdjo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tlvdnhqu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wkdncqrj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lmrkvhjj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dnfvfhcv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3phhfglso.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nyfoqdah.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ujbsvqic.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ipjbjord.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3scsctain.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3doutarkn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zoazrkqa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fohhpoac.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wyirlmzi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cdxeiwyl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wbkhplyt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jpxwpxqq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lsxjgqke.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3syyuydat.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lotijtdn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jxwkqkfg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqzbvthc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzibvojk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dsonsgag.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3guaseyes.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ykpyyafb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ahbgzlqd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3raeomnml.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pzramupv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ddwzhzsu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zuleyntd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sywrqvmg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3doyoavsh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3brpzvkmt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3knitbvbj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rwtemtgx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3salquleq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rkybnsho.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qcmzlvqr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gwgijllk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3renqmbvm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yfmykglo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ukjrkvlh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kzxmdnxq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3eljusaio.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3stxjzlcq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jhrdsqvz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kazgfekz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pagmbmba.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3aoirgoic.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gibunpvp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mwkcgiuq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bcqxnsbh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ubushorl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fgohyfce.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gmmurxjn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lrlqvhez.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hvnwndid.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3epsmozot.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jxziangr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3mclyeqxv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3sizdzcfv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lurvzzoa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zdqgneck.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kyhqmsuo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvppueac.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kccrjgrh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3atpxxkiu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hzdwzeqq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ezulcxal.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nqndfirz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3owjqwgnv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wcfcgqaf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fvydjybq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fpoyrptj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfqcmyjw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3buifxkyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjepjfcr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kcnfrnuh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hwppgsyv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3uqjqukvz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iwrievni.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jwutmjjq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3uzfooivv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jvicvzor.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xpowrlud.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wfhsfthf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bxugcjxg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbgrkmfb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mkhhlwzy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pcgayvqp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jrftgthy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3huyayusk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fsjcmtxw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wuzzngnk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kvvignci.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dwlrgsab.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uieizujl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zgfhuevr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttnnmwln.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ckuvodcw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qddjhpei.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cshfcbri.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3azthtzhk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3upwclfqk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nvapnvie.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zdaollhj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pqxvbtax.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3maoqnfoj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tfvgyidv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3inzasjbx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xgtzcnna.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3oehsvpce.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3regdzwuq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kzdjbwof.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xxqdocbs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qmakjvnb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yrfkpdsm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3trnznqqw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3eyplzfja.html


<!-- 参考信息 -->