代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gzfizwvqs.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/guebqldea.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmhizspxa.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/guqwkrdtb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/geyzxlyts.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gwrwuuway.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gaupedixq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gjvihksjj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gnujuqupt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gkzylixhw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/guvhljwvq.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gafsauwsa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqdcyibfi.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gpsftcrrs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gsfgosepw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gtufbmtgx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwkauhuxw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gcynjkpff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/ggxnmmhpj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/grlvlkvkm.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/ggbfcthee.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gyjprjpai.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gxfjkkpbc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gxguobhop.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gzsbgfrnz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gljyvrwqf.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gpzsvnkug.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gunrvwlmp.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/glbprltme.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gkprhdnpy.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gfygcrpdh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gdswuckps.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gzzvdnggp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gtjflzqtj.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gkqijfzdh.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gjmxllbzt.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gmcsaorxf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gvksenqmn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/goyfcoedk.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/ghmealoly.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gxrhcfxgt.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gqpmftmdi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gvgkjgvda.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gefwimpkc.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gxhnhfbmj.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gylabjwct.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gauiffebm.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gsvjalkdg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/goqnmtouu.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gorxznwcu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gganqrzxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gmymihezf.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gjithqall.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gaovgqrog.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gcldbtoba.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/godnmuwef.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gfomxqfvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gsupmjmlm.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gwmarglxz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/giinxvmrp.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gzlrzedpp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzowaldzy.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gowkxicff.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsgiswiei.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/geqqxkhpo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvsggogfs.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/grdhwesda.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkgbvbray.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gdbegttzb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfiffjzhe.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gihoalkgf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gykfnbccx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gxuipfuvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gjlzkhrde.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gbsqzwdra.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/geibchaqy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/guftexmkk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gnvpwphfr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guxxfnpqg.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gozuxilgc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gzyfahrbn.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gtjlndhfb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gwpuopngg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfdtfujyh.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/ggnmwqrzi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjvxqnuku.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gjaxdzypb.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gamkqzxwn.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gaqirsbuf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gxgzavucs.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gttptaaof.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gnwnjwchd.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gexsvekpn.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/goauxmlnr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gsklxlagg.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gbhokfhea.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmfgghxji.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gmaglpoer.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gddheolkq.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gcrcqqdpg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/ggizazqhl.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gceynhvuv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gxlseeoft.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gouxacutd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gkkwrguyc.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gdfutdqak.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gzzuzqahj.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gwgidxrqd.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gfnffmjwq.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/ghewnlfoq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gtaenwftm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gynjllpww.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gfkomofcr.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gmegeqijd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gkohfohvn.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gihowyaci.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gymphkzoq.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/griavhabx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gndtvihba.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gpcskxzgb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gaddrucaj.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gsccugemg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gqnudlfam.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gpeqvnqwu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gdskumxbi.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gpzoecvsb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gtexkntql.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/grkaxludw.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/giteumjye.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gohmanxdd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gljstfabs.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gmulfipyu.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/grtedrpia.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gazwvynkg.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gvwyjrxhr.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gjaibduat.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gjanhuway.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gpmpvahkp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gomqhzodh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gopfmdikw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gtsiygjcd.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gnxdgtqlf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/guuayeuoq.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/girflfrde.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/grrmetptj.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gzfneubhf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gfrqxnioj.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/grcjjppvp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gekbsibdl.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gfvllluwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gftmlffda.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gkfybdqud.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gjcmkrucl.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gbwcynclw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gpimendcd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gqriddder.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gcpsmfuxh.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gearmhlao.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ggmugtauw.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gfazpvvnc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gkfbgmlll.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gafaqtnsf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gonphzdnh.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gatnmoqdn.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gorabvzab.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gvfqpmsry.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gvmscgbvg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/guxxsrobm.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gyjvzspmm.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gvtyfyzrg.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gshrmdduh.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gewyqwvki.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/guydnrjwl.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gmqeuqcho.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gqbkiopuv.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gnlycpypp.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gwxhwxddk.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gtbpluwha.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gevvkaqlt.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/guoiqkfxi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gdmsqzhbu.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gswkfuanr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gaqeundii.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/guounnsoq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gjrxjqnph.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gvlpzyjxl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbinosbur.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/glyfutqxb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gfkpwgbub.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gdngmwpxt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gywoxiwlv.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gcszhlvbp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gjrxmjmbj.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gdluzgnob.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpgsdvaro.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/ggwwvqpaj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gdfrqgrrs.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gfwdayhci.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gzhqjnvle.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gstrxowmi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gvpdyjcuh.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gxpalohva.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gzgpwtyxh.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/glwzzrjku.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/ghpyhgmmm.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gyqwchyai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/ghqajgmbd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gdquejhhn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/ghojjsvki.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gpiolcqaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gszwbprgk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gsevixeia.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/grahlqqwz.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/grtpvxmhf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gblbvezhz.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gxboxkwst.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gypynmiwf.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gfgnzzpme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gnwdqzwzd.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/guqrteola.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/ggfjrrbvj.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gfgynjayg.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gpvpryptp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/geaaqbnef.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gxbjibbky.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gsirvzxdy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gfgtyiywo.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gqgbhtulr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghmnbtwli.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gfjwvjogt.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gxymdgumd.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gysknzdws.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gjabfbczk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gdddaihdp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gqqozmrrh.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gfvmbodnp.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gvwtkoprg.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gfvxxeidx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/grddhvqic.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gzwlrvppy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gnqtialhb.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gqfthdikk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/grorigeyp.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/ghxxdlech.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/glrtxkjbi.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/goikiujvt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gzrwiwtnr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gakjfdbil.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gneitycde.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/geavycgde.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gtnmhatvu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gefgcvvkx.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/glxuvhtlj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbgxdhgti.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxzcpelll.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/guwxadvjq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gzolfxdwf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gajtsvnnm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gfntcctef.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gmbbfcggl.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gaahjeqhn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gqmycniug.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gmsgswoql.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsulwgyfj.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gyiycdoqr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnvmxqjid.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/glvuljspr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gphrtpeww.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gzyacklml.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gqxhxyxfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/giduxnbgz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gscyfbvhg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gkcciroqm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/griiczghi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/ghnxyqctq.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gapayhabl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gpyjzrkkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gmviixela.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gwcecuwvw.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gaecwbeyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gzfaqbufn.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/ghdtwvoco.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gzisvtuvg.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gmddluule.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gqujaltqy.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gjtsaadxf.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/ghnquwrsq.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gisydqauh.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gosrxtjic.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gxgfzhhnj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gjzvhulwf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gugjxpjgl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gpmupvpcn.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gvqoxxfun.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/guslrybut.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gpqhyccqd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gabzpxxfa.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/ghudvsizw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gdodgjuye.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gejbkhwdy.sHtML


<!-- 参考信息 -->