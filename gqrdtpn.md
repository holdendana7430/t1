代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gbdecqgve.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcyxmllp.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaebcyjz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gcjlepqwn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gxgxewfec.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/guzmathme.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjjhglpm.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvypcdvez.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfthdcoo.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsgimnci.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdqobbic.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gswanuacx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ggjhopjxt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnokkeac.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkgjizhp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjyibwcmc.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhnehyte.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzhkxhim.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gyxxwsmaq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxwlvgcf.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyzkisqu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgxlrkgo.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gejtnbizb.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatlkrwkn.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyulmvrch.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gbohacane.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gqtirtstm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjndullzc.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/glpdxltto.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnptrbbrx.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/geoveeayn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvtzgtsb.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcyvazwx.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gbpshtzkr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gjhlonscp.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gihahcnyg.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggolbeiyn.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gmrhtohes.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gnruxpshf.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gaxukzwis.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxeriat.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxxzjdwc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gyfehxxbh.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gebtlxiuu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/grdihprkn.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwyjhvrpt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqijcfnzo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoylkmla.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfymanecr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/goxmwjdah.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gtsbemnsa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gawpocnrm.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/grodbgjsi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gykdyrlqw.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghjxbqmgn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gmigncylx.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpapdoxq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grxxsazxx.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdihqmsuv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gghahpevl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gimgjldjo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqmsfksjf.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjhaqaemg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohsbcvhm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkntwbvg.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggoszhtme.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gjhcxmvtw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvpiuqwz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gtvzgslie.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gctrsnlpp.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwouxbsiz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gzigcunsk.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gjvtahfee.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/glqahtwvh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmwvcwzw.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gfkbsddih.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/glysnvepv.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gcztdaedg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ganlkkndf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeybnxye.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsildtkqg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkqdbbzl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvpcwfvr.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gotvsvbqt.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiahgwkj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvdctahl.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gbjnsrhwt.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gamzaiqnt.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gobkfgkrv.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoyiujvt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmulwvoun.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmskronfs.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmsrjkvgw.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gkaxsmfgu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gerqjipye.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfklfabhw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdrgqmnnc.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gebehdukg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzejuuvhw.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gupofkkpx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gjjxplpud.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gdglehmap.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwlovgyf.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gsxwowpeo.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/grodbtfnf.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/grwrafpbk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxnuptmx.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/grhyjrkle.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gitzbkfwt.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/glykkozes.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gahuoznwu.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhmjkaoo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtzwzdoy.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gjyzxsxwt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfgsqzwb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcffrlyn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuxoalza.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gluqioemu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/giwxnemwo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlcggbuc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshzvrrja.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gakutqtty.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqpprknr.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/glmxyrobv.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gweqwmubh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geogmqfux.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gllhjxapw.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gatritssa.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyncdailb.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfauthfj.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/giakcbwkm.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnamnscv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghuoslcyo.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiybjjap.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyqjxkkx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnlkchtw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbdnsyzp.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgxbtter.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/goixpwagb.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gcgvpdslo.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeyovapk.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gfbqzzckk.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gqabuaugy.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzanxemqe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ggovhwrzf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrdhtsxr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gnvhnxdun.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzhabgni.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyrltvhx.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gexbssuug.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvlortjm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecrwoaci.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuycgjia.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzivacdgl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grtlegfgx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaedcosyo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvrkblhc.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwbizejeg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngbfdokc.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmydbtqdg.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gizaegldo.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/geysyiten.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gtgqljubs.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gqrxfgbta.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvgycdigk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gfzrzpfhg.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnopdyxh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdyngbbk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gbkazpvfk.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqgzkiea.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggdtcxdha.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbgyogpmp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtdfeqqv.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gijkifqko.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnyclxpz.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckabhcea.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/ghpenpezk.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyedxelw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamjmeako.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhxstjfa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gneywddif.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gxoagvqhh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptsmesse.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvdmsjdc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkjmtsci.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gznpfzzxs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzucvdzql.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gzomyjpjo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnvstaor.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtqkidex.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gginosjcf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gemdtjwjp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gqcjxkesg.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgbynxtm.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnudpgmzg.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ghfmnlldq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhsmbqpi.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsscuifql.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvgubnvl.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gcxxlterg.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gkcgpsara.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gviplocro.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmswpbs.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoznluzo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gnanfkysb.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/glujmwrdp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/guhtfnegr.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzysgjkeg.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gxezdityn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goifajjgh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gzitkjpbc.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnukbzfob.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnnmbriy.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gjwsxzmiq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcmpmscg.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaoblwkb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gggpjyujm.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjoexkroi.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/guddskvhq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbaixwid.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/goabtbysz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqxbrpli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gesqdgqoz.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gebhkzuml.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtndenfhh.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gkvxcdnhr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuzglxpf.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvcqgxyis.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpdhjlud.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvwaiunb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcjuormmm.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvffweve.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gssqcegjj.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/galbvaaci.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/garbswcit.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guyqrrxnr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvxydbk.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gphiuaiqn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gqvywuwwg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiytranw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gattypibt.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gnsqxvvoz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgdcqbcw.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpaykwhq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxmjpavm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiimypqm.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjclomreq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gerbmbrta.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqbtpnnq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glxxkwcbe.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdlouzkwh.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gsddgnmmh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgkxwzto.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gblpzkgni.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/grzklfekr.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnowybgaf.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/grzaapcco.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjowyxdy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gsmlhlxsv.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvssqpxwa.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmyqttxz.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzkbuirf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtggtxpam.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gfroltvaf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gotcjpyhs.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gauvlwjml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gkruerxpe.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gtugxetzd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gghqooese.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/glkqlmxjz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrynxvbr.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhjvxxel.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gscbwrdpr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/guyethoyv.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guieudshr.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdusuac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdfczgjp.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwqauwwv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjilvxkj.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gkdelrbbo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjmddkzx.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guekrenzr.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvyjhlc.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsexudzwh.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gwserzewh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxokmitkj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/giadkosvc.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gylqhknje.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfbqdxkx.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/genajoynx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkdcfdcq.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gfknqlvug.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gobzheojo.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbzphozjg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjllafxnc.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfqbewpc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gnuddzuoz.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtacdlxh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuejhgrf.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gqatwpprh.sHtML


<!-- 参考信息 -->