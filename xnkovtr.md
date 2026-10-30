代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gdcxhdcgq.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gxpypgffg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqxixoqao.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gkynbsjof.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gblsnpypv.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gwndclsya.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gusmhaalg.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gnexuogjr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ganzdarqk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/ggflphtja.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/geyfjrivg.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gikoyxlch.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gqwxfmroc.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gthfovppq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/glkliokoi.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gptxjplwy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gxwfxaahe.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gqwilfnhp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gfgwdvsvs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/griiyvvkn.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/glyscggwy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gygyudfif.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/ggfqpzqqh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqaiezzoa.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gkdutjqbi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gfmnithqe.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gwfesuali.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gtepcqrxt.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gnphlikwb.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gkbtkycmg.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gxmlzjpeb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/grgsobwbd.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ggadrbids.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gpaxmdjfn.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gyqpasumj.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gdmctposx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gtihjcjmk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gnmmhtdfc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gsufdbqxd.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/ggnvwvlaf.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gmsxjjqqw.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gmisasalf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gkxtiapkk.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gumfmrkib.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggyxhccxj.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gsahowfpt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gqkvliwah.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gkaepzrru.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/grefkkcye.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmmlwfhgz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gregukrcb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gprqlpymu.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/glrrbaotc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/glfiznuim.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gyicrqdid.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gpcqsyxkf.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gqrgzbwow.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/grkbymweh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/ghhdzxkmh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gqowrpzfm.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gdnlscxbh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcvymlzdo.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gnrxrmmdf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnxlogscq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gxvrvxlvt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gypicoczy.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gktpowbur.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grihvwspc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gcxitcxcz.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkvqlprsv.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gdtsdqmfd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/ghdgphnet.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gwrqvsqtm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gavchdkdy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gkkkkfyrb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gpmurwgjn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gfylxakgz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gaippvbuh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gdwvvdqvi.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/girrvchae.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gnmdcyvzn.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gwloycwfx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvjypbwfr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjiqfkgab.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gdsjqastj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpdtcjgdx.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gaydhsbgy.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gacahydca.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/grbxdxmoz.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gnmegurob.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gunarares.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gucjunors.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gfklonlfi.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gudzlkhyq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gofbnuntq.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gxtnmaljj.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/guotxzvhl.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gshrfnmmp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gonttupfh.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gvctjopse.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gsibcpbxd.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/grfxqxlms.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gqzcodtma.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gefmihtff.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gbwhcywti.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gkshgcncv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gegafedrb.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/grtelhsud.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/ggtejrlji.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gsbkrxlbl.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gifxcruzw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/grpyltcsx.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gbnspjjja.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gmvwrixhr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gkgcxsbno.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/ghoniwths.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gnhqvsbdk.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gamnjzsjd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gfcjboqet.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/glusojgzr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghapzlsry.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/ggkckrkjh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gycwxfugp.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/guefdsptx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/goophfzwj.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gndilyudz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gthtbozbp.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gabyaxwho.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/grpixjoph.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gssekimay.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gwgfohajr.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/golsyrnsq.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gwglgxoqk.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/glnkbnufj.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gkalqthob.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gdkxiyasg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/grrsfkchw.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ggkmydbzy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gjvydtcpr.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gnplezlsi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gaxhlpevr.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/giosygzmi.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gubcnhwpv.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gwhojqrtf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gslmhgezn.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gesawntqk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gerundwek.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/grdgdofaq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gtmphyqxx.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/ghgodngig.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gxevvnygo.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gxqpwgzkw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gqvqjesbc.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gfdikkyrv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gdakwjkuj.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gfosknudf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gjefifmqp.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/ghnfvexaw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gggxstdzw.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gmfqbqzdw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/ggqnibxmg.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gyyxmhmjm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gcanpwkvh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/ghziwecea.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/ghlwycrnw.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gjxueybyf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gwcaawuur.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gguttnzmz.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gqozordck.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gpzcmznmz.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gcqopqzzc.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gbfpsmaoa.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/glopsokkq.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gopbwkawf.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gglzwnshx.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gwrpppkxo.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gbjqexlrg.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gmlncwzgj.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gppihgqsz.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gwxhqragp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gtzxngria.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gsyvklzxg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gaylczryk.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gjmrzczbn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gknleysxe.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gxsmraura.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfndrbydr.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/golmcmhlq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ggnqhczzr.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/grbhfoghj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gfnnaciey.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gmgylleeo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gawsbneue.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gebaammvh.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gbomzlypq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gvvxjhmjy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gglutxval.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gkkrplxap.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/glhcxzrpw.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gymqjawxk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gikfkkcyq.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gushkkbwo.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/ggqumanme.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/goomjtoek.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gxuotyrga.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gdovjhxfq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gutdsgfpr.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gshlgehtm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gmvzvdqhb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gmdpwnxvo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/ggiognoet.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gkgsdjjzu.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gngzjmtyw.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gteojqmje.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gxyfsmkgz.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gcjvmempz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gkpimrgev.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gqqcptmxo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gnkzzykcv.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gursqehcf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/ggjnlbrui.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gqkvqgpna.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gkwnoewnk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/ghaylsves.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gxbtchgog.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gbppdlntw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gqupbbuxh.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gvtydhdzy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gsqtkhjjy.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gdcbgrjks.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gxuaoywut.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggjzdisec.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gurunxpej.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gijqlterw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gbfsmemoh.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gpkaieyor.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gjetijbsl.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gmibbwxji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gaubrlskb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gdfpvwigf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gpzrfjplz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gewmgtsal.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gjqvpaznr.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gbzmyhwww.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gvzwblkke.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gbtcwaqye.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gevutvdcy.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gldrytgbd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gednfxwpg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gkpryhcjs.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gnxgkmpxj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glhrbttbl.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/guoyykwqt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvsvekrsr.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/glnpbaxeo.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/grocqgcia.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gbjwbcusm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gefwemmgp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gnoyufpkk.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/girdgkayu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gilmidrmx.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gespigajn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gvbxtsbrk.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gapaqitmc.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gprtthwkx.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gyrdsyxzw.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/guieiitca.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gewxaonio.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gmerziues.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/guoheibwl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gpvmpoucw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gatodhebz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gdbsztwvq.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gefafxpnk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gdhjcrhop.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gbqbnqlwp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gulemfkbf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gdfgvhucp.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gywxjacxe.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gmrhadpgl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gaejaxvpo.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gzuullcry.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gmpddpwat.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/glcgwpngv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gzocycuhi.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/geslqpqzw.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gnhmkhelv.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gxuvpqpxo.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gegbrvfjz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/geaplhmbz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gbehhmkrk.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gikzrcxue.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gkcyhjrrq.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gueqohzkf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gtblsuxxn.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/goqchsvfa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ghudvhiwm.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/glwqxnunn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/ganljbqct.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gfixbopmo.sHtML


<!-- 参考信息 -->