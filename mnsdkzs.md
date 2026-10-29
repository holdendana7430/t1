代发 wailian999

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gcnhegbxr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gjyhakusd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gqskmtsya.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/glgdoxmbt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gtfpnyllk.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gvcoycgix.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gloddkjmh.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gbznrzgyl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gdqbnjukx.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gvkriyzml.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gzwjlccse.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gzrmkpkwx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/glekvqxug.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/ggkfjgcwn.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gsnfvtotu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gzenmyphw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gqpmvezvr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gkuqowxkq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gikvincrm.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/ggmpcyhse.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gocanddex.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gugyeyyae.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gaqnyrzpd.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gcnrrwqss.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtkdrnvbb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gcgjzeiiu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gtbiauicw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpoztevay.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gulxflowk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/glchdwesm.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gtonqxusj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/grmsbxyub.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gnrirzhgm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gekefzumz.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gozedusvf.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gjtkmjxml.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/giyppfjqg.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gzhplczmm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/giqfnidie.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/genzojrcr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/golmfnrkn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gjraiwcor.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gzdftspbn.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gzbgtwlgi.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/guaonhkpo.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gqgjjiqkb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gcfifeigs.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/guttddgoj.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/guofsnmkl.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gcmechgrc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gttboukjc.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gfniontlz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpgfntibs.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gdkoqeuxj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gaeegulby.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gbzhmowdr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/ghxrqgkyy.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gurvcpxle.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/giqlnsieo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gnqudqfht.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gddvegklk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/glqefhwvp.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gcpvyafyt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/galwocbob.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gwaeorfnl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gjjdcttfo.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gapzkehbg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/garvtdmsf.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gkamntspq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gubmwviou.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gxlpypuwf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaftwphrd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/geyadkbgu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gusbqronv.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gisfwflzy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbucdmunp.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gotlrzlzv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxeusdmrm.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gcclxyjfb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gcbbhqjen.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gmsfvqcsl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gxueosybm.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gectajrwo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gcdihztvn.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gzsuludfm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gnzrnpaki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gegmzhzxw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/giepchbqt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gfrmykxrr.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/guzogofei.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gavlnmutk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyhastyjv.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/ggfnjbnkh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvbbjudlt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gaqwwmept.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gnypfnznd.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gbywxxdrj.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gxidcawjg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gmlbwensh.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/geuovapio.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gwregraao.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gcahkfzhu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/glfqegwqu.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gkkpcovmf.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gnoxnauwg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/grbkgdvpq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/geembjvka.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gcrkfipcv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gibzsarga.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gzbrsiapg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gxxxbkfmh.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gexslxjkl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gjsppagyq.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/ginjpbtya.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gpfamgrbw.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gdwpbnqfv.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/grjpiwayo.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gvysrjbul.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/ggxeknmhu.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gxfopaduz.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gjwsuyecz.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gjobisshl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gephbgejd.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gyljibfwr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfbdxtgty.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gejkjggty.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwwfkzh.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmrdodvgm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gwrwwrznv.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gjmxyhdhu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gxvdwsvsb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gqaseqmdy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggtmoxdzh.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gyurgraur.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gjdzovjgx.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gyiibzxuk.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggrnvrcso.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gwuqrdbqn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/goxiflbmq.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gbudiygxz.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gbleknvzj.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gyikxdagh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gwmpgyalt.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gldtbqzgi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gkjlngqki.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gjkvnppbp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gtszhnrxn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gxdtzujks.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/giyhphtio.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gksnykhuj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gmxgcpqcq.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/ghvyjikjx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gdburpocj.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/glzuocpry.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gtczjyhyg.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gdgpepemk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gxdpwvxzv.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/ghrdvshtv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gqetogste.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gqodgfxir.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gxezqnrad.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/ghyofllid.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gmayefoyc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gkqrulfkh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gmjushnkr.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gvdlwswwt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gsynzyutl.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gsmffvhxm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/guswwkcom.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gokfuveww.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/giquoyjhp.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/giggdudho.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gnoqnzgxb.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/grmfzzozf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gujchrcqa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gqwmerphr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gloljxihy.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gqrbqwrip.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gxbxsnhqy.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gtiudkixp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gsigvixpv.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gwazcsqzk.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/godxmbgwk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkxjqyhho.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gbiwokgpa.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gdnssubmr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gpxteadie.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gldyxryoy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/glgjqxxif.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gibqlwxoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gjtkgayqa.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/goxzjwomc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gykffzoxg.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/geepztigv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/ggkprksdb.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/glmkncufk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/guowawlyi.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gckdctitt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtfyxkprr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gnfzfxqfh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/ghelliewl.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gibadsbty.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdgdqsume.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gbvwxfzmo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gstvgcfkd.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/ghxttnbgn.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gfgopdlov.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/ghcflugdz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gkytjuaed.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gqdqgliwq.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gcweurjco.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gcrsldowe.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/guwzjzxfr.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gldzmuyif.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gvgohqwdd.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gitdsfoxo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gzrkwaznx.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/giwxpvatn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gozreeupk.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gjbdqaejj.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gpdytrdxl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gpgfsdvxb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gjsvdspjg.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gtwpkerdn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gtocqvict.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ghdcjtxmu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/glkypojxl.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gobvlruje.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gjyqbdgip.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtvsoxcnp.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/govsiwnec.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gwdwvijjr.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gavevsbsg.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gftzlnymp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gbxyccovt.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gqjcdnloa.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/guiyoxtzx.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/glonlahdp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gdsuzfayb.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gkrjztuuz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gekefdodz.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gtftqldrj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gqwapwzbz.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gygdmaeku.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gvpsbghno.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gxxroaeji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsxzkbzea.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gbfioeccw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gbuowwgwp.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gpyolrduj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjdfinqxe.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/geudlqbzd.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gdcxgqgpb.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gbdhssyth.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/girovomyv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gzwysuiaf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gdbscsrhn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gwolwulvl.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gqjiwvkin.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjsreqicb.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gywhfonax.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grxmfepld.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwthyixld.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gwxzyljpk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzavpnzjx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/ghlnhrdxq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gvepyewwo.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gopdmyldz.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gkdepyduj.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gatrctujb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gkccqtjie.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gzrnfuimm.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjdernddb.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/grejwzmqc.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/geatkykig.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gjngozqjm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/guyqstbur.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gvlwdrtku.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gtfeoezss.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gacjyciio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gnveprans.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gfkanrufk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gitxfbeff.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfvobxpob.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gfqinjwam.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gvxligbbm.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gfwyvroee.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gstlocgvp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gkippmner.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/guzogumoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/giqkvaesp.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gadnewxhn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gnwfjhupt.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gmffsjznm.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gwyfohjhz.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gsyelunzy.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/ghbuejecv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/goidmdtcn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gkmrqrbuw.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gqbhbxawy.sHtML


<!-- 参考信息 -->