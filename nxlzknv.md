代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gljtmvsxs.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gsohxztuw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gizqdmrcu.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gknzoribi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwnkkcc.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/ggysctjsr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gupwuvcdf.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gkafgwljp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gzqqqxmwv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/ghgcnnleo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gkrzvmkwa.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gbbdeknls.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gpwkwdxbk.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/grhgaitna.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdxnwhseg.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/ghaeohgec.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gukpauhsj.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gecoelikm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gbcrdiosy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gadhwsiez.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gbptotleg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnqrqwbpl.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gvbkmqmrc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/glblnxvma.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gcvclheze.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gnxgsokrj.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gslmbwwii.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/giwifepbh.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gtzbkmyyn.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gyjhdghfp.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gcikifpog.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gsbicyemp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ggerwjdno.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gdayqlyvi.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gdlnpmdsn.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gupxukdja.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gbtpclfiz.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gycsdmdzz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gcmtvinhz.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gserhntuj.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gwlrpnprh.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gvxxvftyq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gethooktt.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/geeakylsg.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gesrewxbx.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/guokmrtpn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gmcpmbhnu.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/govxrsuau.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gyjsuohnk.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gplzotgph.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gipjdglho.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gxtoontsh.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gaggcktlf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gxhveyoqe.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gtymytbgs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/ghmainrwp.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gffebaojs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/ghuexwbvd.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gkfznavto.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gihqrhysa.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gzelohqkq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmuohdemy.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gzokxmhst.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gepchkmrb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gtlaltkuv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwzsxkcqw.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gotcaqynx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gunhxootg.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gbybqylta.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdhdrkpwe.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/ggjvgbiot.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/goagybgdu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gvdibrmaq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gpxdvrfir.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gtoqyempd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gkoqbcnjt.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gsfsqapcm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gsphzgoto.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gndjjvjxr.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gnbxpfkpx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gtbsiibrr.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gcykutgdw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/ggftqzfya.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glfwugkdj.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/glggzixey.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ganlidjfa.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gholkcbfp.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/grtbbonvz.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gusxzgzxe.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gdvfpwaqj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gxoittrqo.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gbmspyinp.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/ghdrpovpz.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gwbrklzlp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gjhgkffil.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gdslrvwqg.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/giqfcwiok.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gibqrgsor.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gcvgjrcqr.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gplqajass.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsghtlaxi.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gcjyljhle.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gxahkesxm.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gmqeddwxf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/ghqjvggio.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gynljnaln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/glzljpnqm.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/ghgmhyrcm.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gijnkpzrw.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/glegddfuz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwylexm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gwhrkwgeq.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/ghvqipqsb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gcblkgcms.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gytfieffd.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gijpgwmcj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gimzwauey.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gfrzgqekl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfqcplgew.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gersgdiyx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gslycfksb.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/griegfqed.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gkcelmrfg.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gkkszdtxb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gxxpabjfd.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gqgyqxkjd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gxhtnmygk.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gwrwgiywa.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gokptzwrb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gwdyrcyap.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/guprlobnw.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gqtmvsgkb.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gxvwwnztt.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/grkfwzsyg.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gdobrreho.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gwpvbaunv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gsthmlliw.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gttdovsru.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gmvrqmujo.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gzoxysjue.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gravplstl.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gvzkleooc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gckzufpmd.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gqqghvclm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/glqrgzxgg.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gzcsjcsse.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gqarktgrc.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gygpgiukt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gytaahjxh.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gacfordfz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gnkdlgtuc.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gshreaqah.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gzksmomgo.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/giiozshno.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/glabqisco.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gnrwgdabc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gjbwoqzcm.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gxzfnfzct.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gojmfkifq.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gsnaiytum.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gactjewum.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gviuduhon.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gtjscstpl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gsnftfekg.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gvcyqjgkx.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/goxxvztat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gbfchysni.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/giaxazpvf.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/grmzbjnew.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/glcguogcn.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gxfhxdzlf.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/guvamfnqz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gszsfnhwl.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/ggygqykfg.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxkkgikeq.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/guebeevaf.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gsewgofev.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gpyrebnez.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gdllaxurb.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gesqulkyr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gqbczcuqe.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gtaaytcib.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gzdqacopu.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gotimecbn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gugjwloky.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/guxpzrhtz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gjwqcdxpk.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gxvnhrxut.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gekhobbub.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gldgjdgoz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkxyvfaot.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gqxpjdwkf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gmusvsdfr.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gzwrzeidk.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbudimbhp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gorlziyyk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gjzjfywnx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfaafmqfd.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gkbkynytn.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gxpmqkyhp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gtmcorvbb.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/grzkscsdv.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gbvnyeqdm.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gwysdsaib.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gzikzfoww.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gujtxkqyk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gkfifwrjz.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gcgrkyqoo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gtfvdgyil.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gulkbvzdf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gengmcltd.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gmhwxbfdm.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gzzrxizeh.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gjjpklvqh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gqepwxtwv.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/guntysgmr.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/ggwswatae.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gcgivlexv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gruaqkibq.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gkgdxczfa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gsujdflcf.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/giwvftxth.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gimdlobcp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gfxfdeloq.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gelafuhhe.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gjvobdjhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gjxdsgklj.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gzcqvigzu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gywdbibrk.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/glfqnjpms.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gvfceoeit.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gclxwqtox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gsbtbqhbw.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gddtgysew.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gtvnveadm.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gvtekomwg.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gathfgwmu.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/grnkoebyz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gfpnekzqd.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gwivyowfc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gyrfrfkss.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gyzffqgtr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/grrglevhz.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/ghyxxlreg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gkvavllxw.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gkjnrnddg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gjfetttzb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/ggnnlfaio.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gbltxbrne.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gilyeghcf.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gddljhloh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gitrmcgkf.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/grvzcytby.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guzijwdcf.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gxvpgevhq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gdujkieqg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyirwusy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/ggbnpjrfa.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gimozwmwr.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gnytwborp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gsswbydrs.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/ggkteywaz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/ghtogwskl.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/glyhipxiq.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gntlucijo.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gdywilmmc.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/ggxdpihcv.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gzdvbryqd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/guddwyxwm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gbfzugdcz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gpxyapnzx.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gqgqyvrkc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gdevfldxm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gkcaooqpv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gjiilfxor.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gqdmxcshn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gfxxxuqfx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gwdqfwsbv.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gpiihlact.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gbwdxwfpj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gvikiasry.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gcwsaqmuw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gfkddpsrv.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gtukhuexa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gcvrismfa.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gdtwbqazn.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gkuaytijk.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gmzrtgume.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gogyxsiri.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/guroqllrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gbjufyyib.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gvjwiitud.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gpmnbvonb.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/grrfyarss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvkmmbxcp.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gxnqpmzqr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gacbpfene.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/giyjhetsb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gnlczyxqe.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/grxdfyjnt.sHtML


<!-- 参考信息 -->