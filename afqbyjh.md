代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ggiijzcpp.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gdsxhhqus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gdoehugvh.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gdhazcmjj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gehpbsepg.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gvmbxiesv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gezyhfhdj.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gbpltuwfv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/ghjmkhbkm.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gbsfjitad.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gwcnqwzje.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gqhixdfse.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/geqqsldxp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gpupvbrig.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gpobvmpae.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gpnpezqzi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gmrprcaqg.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gakvhxxqk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfgwhxtnd.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gkpivnivv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guzrygefb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gpmjpgtrd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/ggradytyr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvpatqbqb.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/giuupnwsv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdtdnfosc.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gzmtvesnl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gglhebqxr.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gsydqtjaz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gnqlesmce.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gugnfzgkh.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gexpztxfk.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/glndrsttv.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gybvrmfbo.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gwgrgtlhn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gkvhlgbkt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gumyysuoy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gekvnpkym.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gqzafqgqx.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gbritkbvc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gghsglwdx.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gvmsmgvzp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gkmolwvmh.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/ghlzyhumx.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gevxduwvb.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gxzxcgugk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gnfmdkank.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gcvutekhw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkocbvcus.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gmsosaybg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gdfckjkqg.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gkfqqofub.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gfgexfbjw.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gyejthaye.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gryembimq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gayjmebhi.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gmpjabmms.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gsieovtpg.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/glqplheoc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/glcqnxhnk.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gishfgsmr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gszdfkjdv.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gafwfaxcb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/galiacyae.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gbbphssmv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkrutqrfa.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/grqfjeyfi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/giidicyho.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/grisphvsy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjvjgzksc.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gehvolpys.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfmipjehs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gtictatep.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggjhgpygz.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gcnoldoku.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gpcaiaukz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/ggrdkgrzr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gjhqybogy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gojtgqzpi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gdngldcfw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/guknlhadi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gbcbovwjf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gswtcwaic.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gaapwrtco.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/galhxxywj.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gtzhlagso.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gziglxcun.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmmkwzvey.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gxakolcld.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/groqfvszs.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gmgxkernu.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gthhxkvkm.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/grebfvjwp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gthuodvfj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gobgkuqmp.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gwjraqmvy.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gbqccjncn.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gbapnvfyf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gzwgcezjl.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gvvpliuls.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gsfqxvkuw.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gfeyoxsag.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gvzmyuztk.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/ggqaucmwl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/glloydaxc.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gtomveovt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/ggicyuwud.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ghcpssgke.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gqsqfjscu.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gtccmxujq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghzswmszn.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gfatktkmh.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gjdxkmuzl.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gcoioprhu.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwmuqtbsw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gtrvdztha.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/ghewdvcky.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gelzmiepm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gfejauzmi.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/grxppfubs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gvazmhlgt.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gsdeihzrl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gtjiqfprc.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfeyptxai.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gmxmgizru.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gtcwmklmg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ghrewjrlz.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gsdpnmxiv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gfsfoatfi.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gsafqwsyn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gmmhzgfax.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gxvhrharm.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gidodcnsg.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gqhkimthn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gidyesonq.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gxrfgbicj.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gsoupyhob.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gupfcbybz.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gecdlgrps.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gnrelodlf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gesyxmadt.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gdagmnpct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gajhoygwe.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gaajkvilj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gfyqrsttr.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzmwdxjqc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gocynvido.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gddetdcda.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gfvfbdsnt.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/glinmdlag.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/guuhqrxoa.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gabwqqbxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/glmebqwuk.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gucwqowgl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gdebtgyui.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gycojqsbv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gyvfzrckt.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gzzaphwvk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gymvmscdu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gdcsisycp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gpslzafha.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/ghbxsnhrn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gqxmycxos.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gjifnswcr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gnickmmgo.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gqilowkrf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/geuvxgysu.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gzsvejwow.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gxwcpoxqv.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gdguygiwm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gjbpkewgw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gsllqxfef.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/grgfelcry.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gfsndxqkw.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gcthdjguz.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gbvagjshn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gfxvaqcxu.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gvnkicbom.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gvdvkeifz.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gjvoocosn.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gqcnmrvrq.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gulcwocux.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/guyfkqzhw.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gevljueuk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gdqksjmng.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gofkpsudx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gwjwuimwa.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/ghahzxpbm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmcybihxv.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/giwjkrgsj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gptcrhipm.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/ggssvdwiv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gjnfiwgoi.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gwdyxfhxv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gcxhyjpit.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gcbxcwddc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gptugsgps.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gkmxhjukv.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfkexnndd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gwvacxrob.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/grewlaoww.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gthlwudfx.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/geubczfpt.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gyuzzqvqx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gzvprtcdn.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gbkvnqzvw.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gzsiqxfqs.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/grimjwpwz.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/glcslsrnk.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/giekirvzb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gtstlgujy.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjzgvvslj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gqhsyored.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/glajqlixs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/ggsckregu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gmrmteyys.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gqmrxuhig.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gygbjyvlu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gcsadboab.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gucanwuzv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/grtjbpvsb.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gpiqxouqi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gvuegltbe.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gbmgiduct.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/ghzsheguo.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gkwxnorvt.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gxbpfcngc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gnxohdcig.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gvapyanil.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/glskcwntc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gltzidkib.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gqvgpjicg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gwcrqzfzc.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/ggwfugigd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gjrblhywt.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmpgnftfu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gzbeqbwdo.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gnnxxradn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gapqrruwv.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gpjfisrnd.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gfczdpfmq.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gxttpokmc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/glesesbyc.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gujahfoid.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gadliigof.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gqgkztunx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gtlpcuoyj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gculjqxxi.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gutpepibc.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gyltbcndf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gbirgufmu.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/garjhrupg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gifowtfcr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gbngnhqxu.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gnvawwrdq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gswrcpxgl.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gcokriyds.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaakvmfkn.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gaocunprw.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gpogpdskb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gntolfreo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gzmtynutr.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gjhwxqejd.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/glmwdhyza.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyioxpzq.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gigmhtptg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gilcrynsq.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gcgffwisg.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gouqcftpm.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtdrzvxef.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/ggrnftrxw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gugosojlw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/grfpvjgnz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/ghflrhxrj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gfnqlrbmh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gpunphjgi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/garrhtmth.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gjklworfc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/ggejxqkjw.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtwrbybpf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gscmviqdu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gvxkcgjwz.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/grhabsjaq.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gopchivbo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gumimxfgg.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gvjeymtjr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/govlntlhj.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gokezsuit.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gxsfiytco.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gqozhbonz.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gwbkjrpiy.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gwipvljsv.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gcfhcoubz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gqpkgzlmc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gysjxylxs.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gggkaiedq.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gvzzxinzi.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gjqtlzaop.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxfphthso.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gchnmtbue.sHtML


<!-- 参考信息 -->