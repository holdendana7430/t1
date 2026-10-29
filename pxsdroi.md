代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gtnmnrxrs.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gfoxhsbdk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ggcckoypd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gjtalsmat.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gbazjxxuw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gpwhaoiur.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gzlkhuoth.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gyrtdfdwt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxvutiriv.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gyjapmkou.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxmyyqear.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gnqcomsoj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gswizkyqm.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gxfcqkpcu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gvvklmcom.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gbvsjcuot.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gjpxxycdp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbezxmalj.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/glsenluob.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/grkyhyale.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/grixaurun.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/giimdhmel.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gzioxmdep.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gnlfmajvi.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/ggpnmwqmo.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gjybmtarl.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gzrkyazfx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gokxwxhvn.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/grgsgmsuk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gvdprjbll.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gpftjqomg.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/guuvfiibl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gfcftovbr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gqcbboqcp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gshuyoxqn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gkypjymwy.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gcbnocudo.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/grpfagqgm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/ghcrjdmny.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gthryavxh.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gswurvanv.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/goueysiic.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gnrrqidwr.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gfyxmfsoq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gbreshbez.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gaejslfzp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmaaronpc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gjwldrdky.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gntotafum.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gdlstdvef.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gixdcnbqb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gzkwooqer.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gtfncbacn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gncwnqzpc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gjxsimmmu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/giulmtvau.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gcpgbstzc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gtvvmfcax.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gcvhigvee.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbtsipskj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gafuiaxtx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghzmztpzl.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gpodbnvri.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gknnzdpix.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gjrufuysg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmcyyxske.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/genhvoebd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gytwhfynr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gmgkapnrf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gfyeahefu.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gpufentzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/grjhairvx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/givwdsbkv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/guhxdyjhn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxlwpzzzy.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gqtwgmhmy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gktmggbso.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/glmeuiasz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gdsibochy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvrixaacr.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gbsdlomru.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gibzxxrco.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ggkyqrfum.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gqdkeaqjl.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gxerjggul.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gocwfdkzw.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gnexoohwp.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwvvjop.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gpplihkom.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gmjrxlmuk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gyhrqakgo.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gupsgyjti.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gtulwfurp.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/goaxixoqt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gprqxxlcy.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gcqukiktq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/guiogeggj.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gtnaxuhpl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gqylzidks.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gznquudbx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gbeiwtnfy.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gfnyppeox.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzvojsark.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gzmtswudb.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gphsanoxr.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/geseixygy.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gwuwmyiox.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gaywtluql.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/grqurfjpg.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gubpkokjh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gnndedlht.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gngdbfcte.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glmnjoflt.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gtntapdqh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gnzwmakdb.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/guwxtxedz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gliolwpbe.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gkyshydgm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gbacyefpf.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gbfgvchmc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/ggyngnmeg.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gdpuihynm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gkqsnciue.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gjkujodje.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/ggkvoyddc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gkcsfghyq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gsghhailr.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxstuokpv.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gnelyzjxe.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gdrolfrnx.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gvnviptfu.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gjxdepoal.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gmevfmuhb.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gutydvmaq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gldcujcpu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gqxvlvtsq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gsbvgxiqq.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gqemoowtw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gdbvuammh.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gqgspasbp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gxzhoftsf.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gjkbvpacn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gybiwnlzm.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/grynmlsko.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gwvprpzdp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/ghlevqynn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gmgekiufw.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gwmwbkhpc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gptaiwjyw.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gtefrdgtv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gwhennhgv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gqrroqcxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gxocrlzux.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gmwcadmsf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/glgzdpcfq.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gmnnputym.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gyhadixpo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/grxhvzeyq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gvoctqqgz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gwadgljam.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gqecstyxl.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gjxdrkfko.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/govfrueut.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gvhopclzl.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gqgvfdsfr.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/ggubvuydz.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gpwoqzzqn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gznrmlsye.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/grupzdkcg.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/glvmlacbg.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/geermmazl.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/grccqmhjl.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/geqrsistq.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gkvauvffz.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gnudhctza.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gsqcweulz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gmpqmzdtu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gsrkeearu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gmmjmtdwo.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gjkapkcnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gbrlpbguz.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gghnymjyq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggwafjjjr.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gkakzjaqh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gvkfbdusf.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gbbujilbm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwmigmrnr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gameglezk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gqlyeeoql.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gonamiuba.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtgwjrbuv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/goafxlekn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gfscjhwda.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gkvdpypzk.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gruqqzvgo.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gkjxcidzr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/guzuwmdph.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ghjfhfclh.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtihkcb.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gwprnvwqf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gobdogeuw.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gvcayttax.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/guhiwzjpe.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gzdzrxhhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gevumgmkf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gakkwwipr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gwecvysaq.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gnrbsfypo.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gmrjtvult.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gfwejsuzl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/grjlrgwex.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gspynpotg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gryhdsozj.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gkuuizwte.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gslwrhiic.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gsyqvqill.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gbpzjlylz.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/glcvdyojp.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gvyxwzqnm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gkdvsubcu.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gmkfnifwx.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/ghfapfddh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gzhvywyrv.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gnomctcdq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/georagznm.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gxtivcafz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gitqxeegz.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gjwgfhcuy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gkacuaoyf.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gsewuipjg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxrpwtxym.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gpyldoteo.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gccuuzidv.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gwxqgdheu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gydfcamtp.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gjnyfymxe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gajakzenp.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gudpbvxuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gtjqlhnhd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gtdjxuted.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gsiyqzags.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gitjnbnpe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/grbjywynm.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/godzfsamp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpnumnokw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gkpdvljeu.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gtapqbaas.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxkldxjdh.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gpoevgmol.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gixdijkos.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/goanjewtt.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/guerxeceb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gjbcnwojn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gkocbmtrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gjefyybfq.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/ghdxybawk.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gnuvxwdvq.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gawxmgdlv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gzlqqfmob.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/geylehlot.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gzemyvmfa.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gvghekksf.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gtzctrlwp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gtguyevuj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gdchjmsos.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/ggxsbgtld.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gawcwbrmb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/giaaxvhcc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gagfhhjrz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gerdelips.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/giezzcvpe.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gditukxsm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/grdwifxew.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gwxehthtf.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gvbhtojve.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gmnhbtcit.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gthgikxfh.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gvbfmclib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gfvjjoams.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gbwbiwwqq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gjgfhskln.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gzybilclv.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gizbmjejc.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gmorngkdn.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/ggdiscgpg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gldfuigui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gwxronzeb.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gzxgdobtf.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/grhrmzffy.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gpvwkepxe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gyiecmlqz.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gyyomszbm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gqzmbcaiu.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdsnufcao.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gkxkkgbbl.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gftuxhaan.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/greyvjjeh.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gihxnqrzx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gmnqnzbaa.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gbffpykhr.sHtML


<!-- 参考信息 -->