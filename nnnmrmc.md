代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpirwhfa.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuvdehmu.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcoqrooh.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/ggcmiiipd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gzrstzjxr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gtmivjjrm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/ggapvppfp.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumkwwglx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gofydmjcm.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzicaskjr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmmzysaco.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gagfjmctu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtnwcnxyp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gkylzvmvk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gdssdkxqt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnkpmoyc.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwydbrcrs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/giymnjooj.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbcblrkg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gaujqkibn.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvugpmkhk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/govmrozsu.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjhhxyfx.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyztcitid.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjbzwzcs.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvaajuqa.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gcscyteyv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjigdrtdq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gsackgbhm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gigmvvlbr.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjbyratv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmopiiyop.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggbsinhve.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzavvspy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gihdgnuxe.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlffbwed.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhotbblt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjbgcpfs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/goktqxzju.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gtjtyjwkx.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpdlwesc.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcrdgrvx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/guijqgvap.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gpfzsiffb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqgukvhr.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glelgcaqa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwvrulyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmapfkpr.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gvskxyiur.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gfkwoizyt.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctqosurr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gidpztgcu.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gwdvfwasf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/ghkcikcoo.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuwlumky.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/ggawzjdof.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gaefxhrtt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqfppxhn.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gezmhhfqw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwhhajnhh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxjmceuhk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrckensr.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gystfulnr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzirjswf.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/glpbvqvfl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghwbcmime.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gshjidybm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimljfwdh.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/grrmlduua.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcxaihpb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/guqrgspkz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gljvkvfky.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/ghhmrbyke.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gxbrsvstu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmblvltqg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoexnlgc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/glcyqnixh.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gdrzfodvb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhvcofuw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtysfypft.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gilqclugd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheafhlnb.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gcuhdlnmf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgtkrud.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gslhgvait.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gckwpgbzk.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfmfyzvr.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxdxvrrh.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gipknnccz.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghvhwrslw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxtoyjal.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gteffkxfz.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsrlkspn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/geqwlvsjq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbcaishxg.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizwfxoub.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gatxjhbek.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbazdnqze.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gtppbgbiv.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gyunmkcjf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gznsxrspd.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmbrejk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjogpytib.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/guebxbphn.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getfgetnj.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsganhwjw.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gryobpiyg.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gvagqfjck.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gjogfneqd.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guybtqlet.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzdkswzc.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnweeksl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxpmwxtg.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gaucpkite.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsngmcnn.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzkswgqtw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxjlslfxu.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gsrfzxbjy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtftzlgav.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvflounus.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gduprfzrv.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gehraghsf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpkddefbt.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjnspjsx.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypngbzgi.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gtiguumdf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfdqzdpfk.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gerijoitj.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjuxzmpp.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gkivgcxve.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhncuqes.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhhzhzjj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/goordixqj.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gijuoxwne.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gezowaznf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmxbgddb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkmchvhq.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmgtivwm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgvmimxn.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gtotnvgpc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gamqfifcd.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gnjwlazsn.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gikofvwuh.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfkjazopl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gugdvixia.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gjnvkbllr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gbwokhydo.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwzvktoej.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjultvfli.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gzipcyblw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjyyyvsyo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gidfewfgz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhsblvzb.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gzduaqwzk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhqvwfxj.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gagtvruza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gzmhmcjiy.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/grqnifiuk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gibrqfmfo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbpssufz.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmvgtssfs.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gfzwhgqvn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbrbljop.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gttkwypwo.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrkylsqj.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjbrlvys.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gocmhhcla.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gvvnjkymu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwihjifax.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gknpgkrxh.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwtjctuq.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjqrjyktw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfihflzxn.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gmtzxuvmu.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gijznlzbr.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gcxpsxkbn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmdlpyjz.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gkytjhiwr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gebwkorlb.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/geztcgxwl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcktskahl.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzwumgnh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grtmjhmsg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfifjnvys.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnmvyljm.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmaxrrcv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbfnsgxc.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkfkrcle.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxirqzttz.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/givvxatfj.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/garoijahw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gzzsshnkr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gjeelwwoh.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvdhqesy.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ganfumzbx.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzvafpvd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmnferde.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gybwpgsgy.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbytyicod.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvcnywzz.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/guoyasged.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnouqticd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnhtrdvl.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gdjhozhnr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gnymtoavc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdonpkwc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpedlqsdk.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwpmtflf.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxtdkkzh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/goxvjwcnr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlacqjew.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gdjaefnlx.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gwfwlhxxd.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaabwrhue.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntwrfzyc.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghflzzagz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnncpsiq.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsajanyni.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gbvyirnva.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzvmvwrh.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrlqetp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhnxhlns.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsnjgnqtc.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gepwdfyig.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gwsfrvuqv.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gjpeaoedj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvfljutb.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqdyxqctf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gruprnpho.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gubvxmahj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gowugcdol.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomolfqer.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gngsytpxr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfyqmitz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqfslvoc.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/goedhncdh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkdnheir.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtxwfakad.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/glamvbwht.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyqcwtiw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxnoakxq.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseclscpw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggioqiciu.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gekqgonvn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcsredgil.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gpftihedm.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gubygrcgt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gptvfjeqp.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmkjyusdz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvljnqcxl.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnrzaxzy.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gsupumxya.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrhlpewa.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gobvxnotk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gskpbmvch.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gulwnnvzs.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gfcbhgwxf.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gudxiaexh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaxrcukz.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grcfcxkbq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghpzrxhzl.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtoemric.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guagkifao.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvgxuicm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvxzoveh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gghkexbbv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gywjvjiwc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvixjtqxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gskwzvqrt.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gomjelbyg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtkubfgb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmsjoccz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gvcedfrze.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzceijtf.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpywkgigt.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcdyeyiot.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwlecwyl.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyvruybj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcuweiux.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaivjkmv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gguolwwgw.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gckyifaqv.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzidggmk.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gtivcnirz.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/geewxtjwk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcddwtikz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gkidiynzd.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/giwlfdotr.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/grmqmebbu.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuldxqbg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiwuvxre.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/goiqxfqfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhqtlhuh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsqilrub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbldefje.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxhboebog.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gefuvbvxz.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gpjnmwosz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqcqvbxy.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gbllsqquy.sHtML


<!-- 参考信息 -->