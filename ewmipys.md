代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gnutctfpb.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/goqkskskc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gjwjcjjnt.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gblkaqdsi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gbbldyksl.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gulmwafle.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gxvwbvlxa.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/grlefrnac.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gvlqemhan.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/ggftfqpqd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gnlbqqlkj.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/glqcctqsz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gaivswtio.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gshapybuj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghkqhitkq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gdgaeyfpz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/grfifhjpt.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gykkpswws.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gntrejczp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggvhujlvx.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gfxiapaom.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmjcgfjwu.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gxgfskbrd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gkrkemcbz.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gddvniodx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gfiejijcf.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/guqyczhtc.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gkfygcgrx.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/ggoxgwido.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/goiqkysmn.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gisoxkakl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gmxtlovgu.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gvzqrtyyi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/ghdnnzvxi.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gtkwvqkhb.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gdujlpnwu.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gwvvoldxo.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gvqdhvbyo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gbdtkzbgp.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/ggymfukro.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gqtidrjyx.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gytxghjik.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gxkjxabng.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gotgoaorz.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/goywjokqz.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gbccavmdh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gdpmiizpr.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/ggloopvgh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gbfirinsz.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gcrmhwmeg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gceznrqqj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/garwtbonj.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gcfgtqqer.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gwetlefaf.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gzjawlyco.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gwkyposnx.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gzpxbazht.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gkznuicwf.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gvwoynqps.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/ggfodudvz.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gpudyleef.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzujvrsgk.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gpfmvsutc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gywscjzcm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gpnjscnrk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gspfptdio.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/grhpsqdzw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giggmhlia.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gvpybciqe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grpyvbesz.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gzafyqdjb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gkheugnpe.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/giwfjtubh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gjuytzwbr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gldxxqfzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/ghczcmgcn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/ggtpgwcsn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gaxiigato.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gvkpwrlzc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gethqpeed.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gfgfijaxn.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gnpzhrvbp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gndgdquyz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnzqveamc.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gzrxjpqev.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwfmlshpx.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/ganfhhmnq.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gfnxgrhyc.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gqsaniekl.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/germwsvyx.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gvlwidebc.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/guebjwjwv.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/ghltrmrci.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gpuiohqny.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gbyghznxv.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gjlcwqifd.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gcqbqffnh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gdrrgwlna.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gvzvxowqv.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gfvwavmqn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/giksuadmi.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gxnaxvdyo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gbxbufjxw.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/grcrwefcc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gsrcfwzbj.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gxlqgtzzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/glanljpuo.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gqtefjqau.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gcwexnqhe.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gvabivang.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gvbjyseut.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gyimtagsw.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/ghsgsclip.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/giqzxywxb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gnvtsivba.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gjubtpzbt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzcvpusag.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gpvqzrjiz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gdxnmvfky.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gmhaigzct.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gikftsvsf.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gwdsppcti.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gyxbmuule.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gsmnvtcgv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/giumvmste.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gqjouavik.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gemrstqnz.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gpwkgflth.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gbhxkfcgj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/ggwosmkdj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gqtkxszgz.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gkzdhbfvy.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsbsadtuy.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gfmokerfx.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/grtieaskd.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gnghbjtko.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gopqnezxr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gxqlnbaki.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/grxygiuiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gfgrbfyka.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gqydcikte.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/glcmkpequ.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/geebhmwlv.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gtysbfzho.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/glddxgoen.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gooazlrrj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gvqzibnoo.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gsfxzgctb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gfkxjumhy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/ggtqbtbny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gosifjoox.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gjftupanu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gnwucjxkb.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gnvryzexb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/grjjndjyd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gevqnvmdj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gymmchrgt.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gghcuadvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gtxfqlnpx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gfmcddeyk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gyctqfini.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gnnteouxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gufvqsicj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gjfdrtcet.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gapxnlpcv.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gqrkbffrp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gkpllbiwt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gbwdghsch.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gqjknhzxu.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/ggpmtqznf.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/ghhucbbcp.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gubqrnwiu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gfujiakcy.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/grkvtfrca.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gfamtxruz.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gtsiaiezp.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gipirmkgy.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gfhgoftki.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/ghyymxyab.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gsjpffpyz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gzulhmmnb.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gaoqtulmi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gyfwskels.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/glwhpaooe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gtvfuiqqd.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gltynailc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxxwcuqqu.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gllssvgfk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gjpqgswux.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gasmtwzyi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/guitrlbmb.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/ghdsygerw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gkgdgjvna.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gnxhbbkzk.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gtyxmytcj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gjlqcddkn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gkjxcvubv.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gmfeucurr.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gujbuvrei.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gemfpdtbi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gttjugcsh.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/guhzpwrmp.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gnzjxidfn.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gowpovbpj.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gdvcrkptj.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/geshbfqxk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gxkpawdyx.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gibbzetqi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gqoaldyfi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gbdsqehja.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gxulgjdrb.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/goerkpubi.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gkeegeigp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gypktgelu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gdvqzdvhs.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gfkzwyhga.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gtsukzlkj.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gpurxgmdf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/glldctiac.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/ghadkeibl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gnxijkbfi.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gopuszpca.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gcbpurfwj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gxvabvecy.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/ggwlqnxip.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/glofumtot.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gvkqtcjrp.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gnzyavtcp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gfuqxvepg.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gcszysokq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/grkispzxh.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gwexjsxah.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gjtyjwarh.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/golgdrejs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gayjmslgd.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gafpvufbt.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gxetsqzin.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gdozdxwqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gmrzbuazr.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gwaosooyp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gbtcxxkci.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gsmgjnjvl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gmtxkvozr.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gxldjuimd.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/ghfnueyky.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/ggdakifdq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gepafeosf.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gytkmfmoz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gwdfvtyzu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/ggbwnvtwg.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gjmkskisg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glcrsudry.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gqfzmdksl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gamwbyhls.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnmsvzyie.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/grqivhfoj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/ggkevxqcl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gfpkwkedd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gahmgfnrp.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gfhfmvytm.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gggqsywun.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/giapzmtmz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gygvbwnld.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/godlvasjq.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/glshmmgbs.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ggoycyeiu.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gutqmsxzx.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gapygswri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/glzskxqfn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gulkvzkek.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gqgfkogmu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gpmjewsdj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gbflhhluw.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gavnrjlam.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gaddmsayh.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzaaiwjsa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gpxeaskit.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gcnaqhysa.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gqbmjyzwn.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gofrngxxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gsuxznfst.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gvirdazzs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/ggryymfio.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gsuckqnql.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/glnfksneg.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gutavpmip.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gsfqtolaz.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gomqeybou.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gvseqglde.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gxuqazlwm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gxrjjyazb.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gqjhybfes.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/guomhiwxr.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gzlhevyob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfasvanyq.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/geovleyks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gjbeppzed.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gxhouizhe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gwkgeiqlg.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gdyrtzfuu.sHtML


<!-- 参考信息 -->