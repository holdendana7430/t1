代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gabexpiyd.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gfrdopjld.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gloqpdour.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/geigcorka.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/ggicmvbod.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gjeuvtqqo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gmfpefqvx.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gduwdgrmm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/geinpaorl.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gxareqxtv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjpgqbvsz.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/guzymagpi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghyrcpyyq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gwxxlpoxk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gdzdxjgjk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gorzmmhcp.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gldbcmilp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmffeiqfw.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gzjorrlea.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gzvptpbyz.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/ggbduptri.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/glladeltw.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/goractykp.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gdwypauvd.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gfainouwt.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/ggdlhfwbk.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gbwwplxhn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gmjnrgxfp.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/glhfmygkr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gxuwduxzr.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gleblerlr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gkzxfeuvn.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gywgkvjxz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gnxppucln.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gihqukyeq.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gebydiucm.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gtjkhaxgn.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gbcffswej.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/ghgjdgycf.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/grdwzyvzy.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gomqreprh.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/grwmhoryg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gtgpgwmmb.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gvwfdbuuf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gczxstmts.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gmywvucal.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbjfgyqex.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gjxqrolmo.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/ghapunlkh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gfbfoatqa.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gojmquhai.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gxllckbsz.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gpqaedpxv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gbxirhjke.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gzkkgmnbt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gcofhkswn.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gznsfrlge.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpbizyoem.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gfezctnbo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gvsifienf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gdnmwwgzh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmnqyxbzb.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gopdvxniw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gciqwkank.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/ggnubgqqm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gezsfwxsp.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/grxnhdikb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gjxhjkkxu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gftxtcfae.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gcuxycjzb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gnhisdalu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gzoehztrq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gsssiload.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gxdqejnuk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdrwepyqh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gwyxbguaq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gztgipulz.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gudqtbccb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gaeijlodw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gydgywafs.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gdovnhyry.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmmyaudow.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gsbxngjxv.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/ggkvsaxnl.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gpjdiqumy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gecaabbgu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gsoczbhlv.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gqdbdamrs.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/glaqacyus.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gtfvgqfid.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gfryqyyqe.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/glxlvpxge.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gwwpnazsj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gqyvthxfz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gwxcocdil.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gyjdfjgij.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzbhwop.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gumcwwbhz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxdnzwtqa.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gnakgdnuw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gjxwgdgkn.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gsxvicrqi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gchftpkcu.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gupziovsx.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gyszozyfa.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/glwujjmyk.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/ghnzbjkyx.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gnopvuufl.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/giyorfzma.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gkumyunwx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gaqukkfmz.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/goqtedxxv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfhgxcvfb.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gbcyqvrxc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gszdtoabb.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvklofcad.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gsxfncnzf.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/ghihbmjfd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gtkqgkict.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gzcjvydpu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gldgzpqmb.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gvxrqbpnm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gfijjvpca.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gtgvqwhym.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gzlayqsdx.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/guufngsna.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gmdajpvrq.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gegpnrowh.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gtqsgmjai.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gqpeeaftj.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gmjizfvhc.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gouyrszus.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/giadgiizj.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gbaonunsm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gmfrjpzau.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gzmdptprk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/ggdeondjm.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/grkkdizdf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gfrngebuf.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gxwqiatys.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/glihiiiph.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gekgihthj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gknmbcnqg.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/grvrqemqq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/ghtwwesja.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gvnofphdx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gmckcxsgy.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gdnntlxkb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gdpwmbfox.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/grbtdufnd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gvazolwyp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gkyewnzhp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gpziovgqn.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/ggqkpienw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gsvwlaubc.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gosrvzzct.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gpyfkydrt.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/goedjvpyf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gdjucebla.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gjjleidxg.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gutyjwdim.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gdstrrrzq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gykaoerty.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/giinckvrl.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gdgrpgvhm.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gfdddnsvt.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gnfhzklve.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gixfxmrek.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gxyoomkog.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gwjfvaptq.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/ghmkbxfzm.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gykwxoiyg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/glnaitbmo.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gmqskubib.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gqmskzjnu.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/grtupmvmc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gcxnequfv.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gpflwivbx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gsbbeuiox.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gzsgiljgb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpngvxpgj.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gdmxjvqsv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gctvzatcw.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gzkynhqgq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gyhisypnz.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gjigesvlx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzmrsvsfc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gueluykkp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gtkqgfwwd.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/ghdgfyatl.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gatrbefob.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gfacacmcd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gerhlqecr.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gcbumqkqo.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqwexclok.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gjqdaqjpd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/goulzofdm.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/ggkyetjoa.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gnkasyjlz.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/glwuzlysj.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gauekivvp.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gavzjzpma.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gjgllwobt.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/ghdnqhldq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gyfdtfkdf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gyjgcnvmo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/govyxtaho.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gffjhjcwk.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gnqciqbmw.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ggfkwmdqo.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gcdfxeyeg.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gyrtcsvfl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gbarfoqdc.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gjrbejfua.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gfxsclvwv.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/ggveghbmb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gpjmumvab.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gabathxkj.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gujxltdwp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gugiqjigc.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gpekhayhf.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gfquwkjnx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gbbxnpgct.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gopyxyemp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gnrtbrxhn.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gqrcwvhlw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gmaezuuya.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gbwzoifbd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gcixtgvop.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gxpajlqzl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gsddqwtdr.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gcmohgaev.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/goyvhyrna.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gmmwvljla.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gjyewkiot.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gwyvhjgmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gmcbskbdh.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gjwkoijkb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gidnurqla.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gqfqjyrkw.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gfnrdozcp.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/ghjigpgby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gwbkrydvo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gzbdytjsz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gtspbtjub.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gdjwfivkr.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/ggylyjgcr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqcbdvfpy.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gjxvczpzo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gblamtfir.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gnybuaffi.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/glbgaekjk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/grgyzggnj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gflovwbwj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/grsgufaqp.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gddlyuoks.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gpdpuxyfj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gyrfaekoz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/ggfqzvsdd.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gnneeeikg.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/giussexmn.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gikhpegez.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/glvsiyind.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gswkayxhl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gabrsswjs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gatwxtaib.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gnsnvtfkv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/getmbdxnv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gdciaolfs.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gwefhurkw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gzgffdldm.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnlyzdzkq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/govdwvjys.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gmslszluy.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzssmizes.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwnfrdazv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gedzuygrf.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gvhtelupy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gjtpvsuvb.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gffiwnchw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gwjhnvdwg.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/glekebbod.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/grqlxzuki.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gythddkro.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gckhvrxyu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gaimdrsbd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gwdtzqxpd.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/ghbfoofcw.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gnpjondyd.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gaqlxavsq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gqrvuyxwg.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/grcmkvtih.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gtdmfyhpe.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gntklrnet.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/godkubxeg.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gbnuanuuc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gfwjmqjsz.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gbfcrbvij.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gptrmyzwj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gqrnybhty.sHtML


<!-- 参考信息 -->