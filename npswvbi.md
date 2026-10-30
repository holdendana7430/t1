代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/ggukfgcfa.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gkmtmfvbo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gajrlbxdf.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gkpjduurc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfsphzsra.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/guvtgvhpw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gpbhobolm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gntcahnig.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gqggesaso.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gzddejzxe.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/goazolkzs.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gpvpnlkic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gytktzdhv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkmovwm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gjlssrfvq.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gdmmbxsmw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzrxeaagp.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gungvtfrc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gchzritqm.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gtjlxzwta.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grxhpvgjn.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gnnzbsxyj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gtxhqvejs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxaydrklj.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/glvtouzrq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpezwookc.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gqhbneizw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvqizvsyc.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gdiaqgusi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gbywguvti.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gunwicsuz.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gehuguuqj.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gyalhxqli.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gkgcttumn.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gijbxebml.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gbwpyfdwr.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gvnremsnm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gjpljzlto.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gosyunxjf.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gxmpvggvw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gksyumlzh.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gmsnvuwkl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gwxwjvtnz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gzpilwutc.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gygctfzen.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gqekpvqfs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gnjmcvftf.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxdnakv.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gcmfesefs.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/grbpzgurx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gvdgcwnyw.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gcbmxbzfp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/ggkxustlo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/guvrjlpur.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gigbvgqqu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gcyiztdfm.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gwqswyssx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gqaxuylyq.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gkvndxkol.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/grbmejxqm.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gpfrvocqj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gorheqmpa.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gnkxxijxt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gdqqvdixe.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gqdtxmnas.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkqhydhbu.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gcphepars.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnrbeoewy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/ggvxuqzyl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glcwiguzf.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gmpucdjzf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcfygdjbg.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gvxzxrghc.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmvyqqllv.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gghoiitjz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gcyxyclzv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gszoecmtk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gyageofeh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gbsdahega.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gbeatuqkk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gcufjrvwz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gkbmetuck.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gheilsidl.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gqdndcrus.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqackrm.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gqtblcgop.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gmheabuen.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjrnncoou.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gjatilawx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsywtkwtb.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gqhoabjgv.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gypsoxwdu.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/ggsjqylik.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/grzuztigo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gyuwfdfws.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gsoekebsh.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gnncgdgkz.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gmxkaowug.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gxvwynadn.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gbzwngzld.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gngaqnvnr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/glbnuunaq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gylmmwmsh.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gaikzjfcf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gmwhflhez.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gwihsfwab.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/guxzihymp.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gnqciunhp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grvnmidla.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gvcsrfdsh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwjwbwkxl.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gbgqddpjb.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gkfzahgxp.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gcngnlslk.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gsdiogsut.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gislvrxio.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/grigqvepg.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/ggzokslrn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/ghyfsudox.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gqqtntsui.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gqjdmycjo.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gffrawpub.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/ggdpvizbw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gynrpzimj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpaxzotwp.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gyuphrtjo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsiherzwu.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gapocsxer.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gvtbyzewh.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gtwnucuht.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gsictoaiu.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gslqbgvtb.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gkpunsdmd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gvpsyioko.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gzbjtphik.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gyejqbdee.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/galawhmrv.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfyfcxgrm.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/ggltyljkw.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gklxlruxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/ghxhaioxl.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gohumycqd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gravpweqr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gvocnccxz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gixyxgtxb.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gcehfjygl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gzbfxbyqk.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/geaiuzstg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/graartgxx.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gmoaxnhpj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gznjhnejp.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gygmvfofh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gizlvzzfq.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gokggymza.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gmjkwxqod.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gsaylvcxl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gauoquuex.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gcpfefxck.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gaxiuiwqv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/ggoljhwqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/giglgsbog.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gffzaxvfd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gxpbusdel.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gnjzvyysq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gfakxifom.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gnhsqkrir.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/guxspevrw.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gjneuvvvl.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gkztjdwwp.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gybgutsfb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gyewdfvfa.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gcnjswrpg.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gvzrdhnqf.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/grbvgfeak.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gnptorypm.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gxckqulaa.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gkpslcimx.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/glvcncbsk.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gxdsmsgdr.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/givkcidom.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/giyndzbjs.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/ggjuclctl.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gjnbplnhz.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gvrxibvku.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gakqlyioa.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/ggmxduwtg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gyollcutm.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/ghsudimks.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gspghgbzt.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gictgcqcc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmdxgsyaw.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gsrfewian.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/ggrcudpup.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gegquptue.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/goocmhana.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gucsnzhvk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gthuxwmga.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gisxqnoel.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtbsozzdc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gkbvpjixc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gvtwxcwqu.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gomqgjziv.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gdgteacqv.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gatxuhusa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gnqhubxcs.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gtqjhotkv.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gktinatrl.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gqmxhyrkm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gkziudawq.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gtydwihuy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gbzznlzrd.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gyejzdoje.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/getfcxscy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gryklffbr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gdoytjspl.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gbwtfrowu.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/ggzzruwrh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gcqgzqznj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gbnayxskc.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gwdraqwhs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gphngyvnk.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gvhyveubl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gseufyqqd.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/ghxnewuhj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gcpcvwsvy.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/grienhhgo.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/ginhleytj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gnjyabzpu.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/glwwcfnna.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gagolting.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/grwqbkpjm.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvvkluvrv.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/guwixcsbk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gkqbqyskm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/glkfmstub.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gmnrcvpek.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gqsozdjaz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gnnbkjdmr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gxttlffvs.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gjagufbnj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gvojrupyl.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/glaqcmbsj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gacscvhxi.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqesfcl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/ghotdhfdy.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gdnkzumug.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gwbwthmse.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gfjzoqktr.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gaqefddvk.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gfurfckup.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/ghuxvsxiu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gqqfvgthl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gtzyvgofo.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gjlmcbpqd.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gkafkdbyr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbsvwmrik.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gnuymrgsa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghwmvtane.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gozxgnsog.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gigiilsau.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gjywvusjd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gmqpchuaf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gqbxqrnzs.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gvenhamjr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwuglmiv.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gwydwutpg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grqfnnwpb.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/ghakqqywr.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gvqplejex.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/giuuddgfw.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gmjiukgge.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gtasxxeph.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gizauemqa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gzkkifagb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/grsrewqgu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gpkmmkczr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gkaymridv.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gjuefhyco.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/geiigcsiv.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/guzhrvlbu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gqjmgzinc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gldyvjght.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gnfpjzzjn.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gxooayseo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gdhmegzie.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gajkemsbi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gmhrbbryk.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ggblrjtgg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gvvewzbyb.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gwvxtkwgg.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gntecpiys.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/guipvbdku.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gavkolavn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmwerymsm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/geserwkqq.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gpjbknoyv.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gfufepchh.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gwearewej.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grvjhxhir.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gmdcagxvp.sHtML


<!-- 参考信息 -->