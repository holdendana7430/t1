代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nwbrower.top/gtfdkfgtaw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj202588.top/gtwpdkrkii.html

[Q39] 自连接（查上下级）
来源：http://hz.guowangkeji.top/gtzwmupquc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hysaishi.cn/gtckmmpqbx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guannengcc.top/gtzuzfionp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sweek.top/gtdhzuaivt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tianlin.xyz/gtxzdkqche.html

[Q41] 多表连接
来源：http://hz.fzhhl.top/gtpenehdyy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtlrhwtjqt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jlsjyb.cn/gtpdkasijr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnxiangtu.top/gtutjsflay.html

[Q42] 连接条件附加过滤
来源：http://hz.aibaodan.cn/gtvvtmpzus.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ppjwa.cn/gtcfuxzxym.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.andypj.xyz/gtesssjmtq.html

[Q43] 标量子查询
来源：http://hz.jqgufenzy.top/gtistlpeax.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtdhhlvnob.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtlwjmvkdc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yonumen.top/gtpawqmjis.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gtvzlmuqme.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtlvtzoota.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gttjlrfjkj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtkoeddokj.html

[Q47] 与平均值比较
来源：http://hz.xylfe.cn/gtiygpcwkx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtphktrano.html

[Q48] CTE 公用表表达式
来源：http://hz.hongshengwenyu.top/gtbakvpjay.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhiwuduotai.top/gtppiuhaon.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtualjxcno.html

[Q49] 更新单行
来源：http://hz.yj202588.top/gtignliuxe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtcygyckcr.html

[Q50] 批量更新
来源：http://hz.hnxiangtu.top/gttdupucnw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtazdqtocz.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangtech.top/gtxsrzoxmu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj202588.top/gtghfvtgyl.html

[Q52] 删除指定行
来源：http://hz.tian-w.cn/gtplxsthlr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxinkj.top/gtfayedltd.html

[Q53] 按条件删除
来源：http://hz.xuanzx.com/gtjzbxggov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuxming.cn/gtmpcydffq.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtbmehkkfs.html

TRUNCATE TABLE logs;
来源：http://hz.dianchejie.cn/gtgysbgqxv.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtlhdgilvm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.redwolf501.top/gthtgnyrsk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jianghu66.top/gtukildlpf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fzhhl.top/gtgcjhnvas.html

[Q57] 行号
来源：http://hz.zhiwuduotai.top/gtsfcupyyi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtcpzfnhjt.html

[Q58] 累计求和
来源：http://hz.jinqigfzy.top/gtymmgqkjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtnoioivlm.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtxbrhpzxf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtnoxkxvlk.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gtzuxewpel.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhaomingkeji.xyz/gtfitqerdz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtxqbkgoto.html

[Q61] 移动平均
来源：http://hz.ydjk.org.cn/gtjutzsupw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fzhhl.top/gtpbplnaix.html

[Q62] 分组占比
来源：http://hz.316326.xyz/gtkkvybgua.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtdrvnehgt.html

[Q63] 开启事务
来源：http://hz.shanyushiyangkeji.top/gttvkbdrbm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtmbecvpca.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gtzdixthcu.html

COMMIT;
来源：http://hz.andypj.xyz/gtkbnrlxuu.html

[Q65] 回滚事务
来源：http://hz.zhijiandao.cn/gtcnahtdgp.html

ROLLBACK;
来源：http://hz.quarkkingdee.top/gtiqhlirpg.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtiamxrngm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtquyeynct.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gtbtgdogom.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtkqlcicdm.html

[Q68] 保存点
来源：http://hz.52xcode.cn/gtqgjnhafw.html

SAVEPOINT sp1;
来源：http://hz.ybcxt.top/gtigkzkfdm.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtnplxhdrz.html

[Q69] 查看执行计划
来源：http://hz.cdnleiting.top/gtknwhwdgw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxuanxn.top/gtnsztpaag.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangkeji.top/gtbfftnhtu.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gthtxqzstf.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtaphyynhr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.haohaochexian.top/gtwuslwioe.html

[Q72] 查看索引
来源：http://hz.hywenlv.cn/gtotzdhiiz.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtasqgauzd.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtzwazqrjs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.kuanghao11.cn/gtftgfbfaq.html

[Q74] 强制使用索引
来源：http://hz.pengpengdd.cyou/gtrcesqcof.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtqqtszoap.html

[Q75] 日期格式化
来源：http://hz.ppjwa.cn/gtetgpmxkn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yangfankeji.com/gtduujeagn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hysaishi.cn/gtayvlpxeh.html

[Q76] 按天统计
来源：http://hz.jinghuilouyu.cn/gtcpajxwtb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gtmzzkzlam.html

[Q77] 时间加减
来源：http://hz.zycfv.cn/gttepjiksb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ppjwa.cn/gthvryxmza.html

[Q78] 当前时间
来源：http://hz.316326.xyz/gttymeotyc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtvpgaueou.html

[Q79] 字符串拼接
来源：http://hz.xinyue.icu/gticuhedxx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gthfnayvgc.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtscgayfbe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.c1oappe.top/gtywqbaeby.html

[Q81] 字符串替换
来源：http://hz.zycfv.cn/gtvqqwfshn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtfcyqcgsk.html

[Q82] 字符长度与字节长度
来源：http://hz.yangfankeji.com/gtnonpqelp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ybcxt.top/gtyuegeddy.html

[Q83] 大小写转换
来源：http://hz.sxryk.cn/gtfbbmeabi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigufen.top/gtpinlwbal.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtovsjpcre.html

SELECT TRIM(name) FROM users;
来源：http://hz.guannengcc.top/gtvknntxfq.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtsgehzneo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtubxiatwt.html

[Q86] 读取 JSON 字段
来源：http://hz.cqqwz.cn/gtqiqpkijh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangdashe.top/gtbkgxcgdw.html

[Q87] JSON 字段做条件
来源：http://hz.jqgufenzy.top/gtifuzyodw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtzbzmpqlg.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gthdgjqfqf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.quarkkingdee.top/gtyuygnfxj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.316326.xyz/gtheurrulg.html

[Q89] 判断表是否存在
来源：http://hz.zdqjudy.top/gtuucmwsup.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xziqi.cn/gtghvoiltz.html

[Q90] 生成序号列
来源：http://hz.xziqi.cn/gtshzxxlca.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.redwolf501.top/gtvokpsmat.html

================================================================================
来源：http://hz.fzhhl.top/gtqhhuunjp.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gtvasutcig.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwkhprvkd.html

[R01] shebang 与严格模式
来源：http://hz.birdmap.top/gtbnanjjgo.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtvdrvtvjz.html

set -euo pipefail
来源：http://hz.pycfn.com/gtlajsyiqn.html

[R02] 变量赋值与使用
来源：http://hz.redwolf501.top/gtrweuxvzx.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gttptihggt.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtxvccgfpk.html

readonly PI=3.14
来源：http://hz.yj202588.top/gtaorwrbku.html

[R04] 位置参数
来源：http://hz.chenzaomai.com/gthuglfuzw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gthkqydlds.html

[R05] 参数默认值
来源：http://hz.sxryk.cn/gtaoxfazyt.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtkqzecrkx.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtofhpxbtv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gtehhzqywl.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtkpvdpzuj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yonumen.top/gttyryrnyf.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtqyjazmev.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dianchejie.cn/gtvoeevtdl.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gtbghlxuwj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtqywogtwp.html

[R10] 正则匹配
来源：http://hz.zhiwuduotai.top/gtflndftjf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shuidangran.top/gtooomqcqk.html

[R11] case 多分支
来源：http://hz.cheryme.top/gtpbrzkvnk.html

case "$1" in
来源：http://hz.ehwqpu.com/gtbpcnfiol.html

start) echo "启动" ;;
来源：http://hz.xinyue.icu/gtfgpsfdqd.html

stop)  echo "停止" ;;
来源：http://hz.haohaochexian.top/gtrdeefiul.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtyzkrfltf.html

esac
来源：http://hz.shzxlz.cn/gtqxmhzobh.html

[R12] for 遍历文件
来源：http://hz.xuetiantiany.cn/gtlkraumsa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtsxuxvewm.html

[R13] for 计数循环
来源：http://hz.c1oappe.top/gtbckyrwsc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangdashe.top/gtlfrmabez.html

[R14] C 风格 for
来源：http://hz.yj20258.top/gtautgkwkk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gtajieiyoq.html

[R15] while 逐行读文件
来源：http://hz.hnqzz.top/gtruefycai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhaomingkeji.xyz/gtueutlxum.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtcsisndcx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnxiangtu.top/gtbvtcqrkm.html

[R17] 数组定义与取值
来源：http://hz.52xcode.cn/gtvlbaltsc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yangfankeji.com/gtmpksjkpq.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtrllbmewf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenjidiqi.icu/gtkwhdtvmk.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtprlpdyay.html

echo "${#arr[@]}"
来源：http://hz.fzhhl.top/gtirmuvtsy.html

[R20] 关联数组（字典）
来源：http://hz.sufxvd.cn/gtxunzphwj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtimvguneg.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gttmzgokew.html

echo "${#s}"
来源：http://hz.ydzc1.top/gtrqmnwdnd.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtlvcstzuj.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtzcwzknln.html

[R23] 字符串替换
来源：http://hz.9152youxi.cn/gtdxzvrpqy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gttpqaegxj.html

[R24] 大小写转换
来源：http://hz.tianlin.xyz/gtpasanqdm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gtgbfsuorq.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangkeji.top/gthjhmkejh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.316326.xyz/gtnhvngmvo.html

[R26] 命令替换
来源：http://hz.zycfv.cn/gtlvooudnm.html

now=$(date +%F); echo "$now"
来源：http://hz.aizwys.cn/gtqcijngwc.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtoixzycwa.html

echo $((1 + 2 * 3))
来源：http://hz.nanxinkj.top/gtwmqxdwwx.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtspjckwgd.html

echo "scale=2; 10/3" | bc
来源：http://hz.daria6918.cn/gtaqczhzcw.html

[R29] 定义函数
来源：http://hz.cdnleiting.top/gtdrjpgrqu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gtcugpyeon.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtrcsnidlp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtyuheqgnr.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtqxnxpllx.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gthrxstfdq.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtunivzelx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hysaishi.cn/gtkcwmorrs.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtonkgnhsc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gotoacloud.top/gtntfvnkwt.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gtooynsvic.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtajfhudaf.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtjofeehfh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtgvmibnoc.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtxhfqityc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtskxrbptm.html

[R37] 把输出赋给变量
来源：http://hz.pengpengdd.cyou/gtmmktixru.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtdfyntfzx.html

[R38] 管道串联
来源：http://hz.pengpengdd.cyou/gtbegyjsqr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gzhubu.top/gthajpqwrj.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgufenzy.top/gtugxflhgw.html

cmd > out.log 2>&1
来源：http://hz.aibaodan.cn/gtrvgpewwc.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtuubtewbf.html

echo "log" >> out.log
来源：http://hz.yongpay.top/gtrgeohhpm.html

[R41] 丢弃输出
来源：http://hz.jlsjyb.cn/gtuojatkhy.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtybbtjnsa.html

[R42] 输入重定向
来源：http://hz.yangfankeji.com/gtgqhfdbne.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtaqlbfged.html

[R43] 按名字查找文件
来源：http://hz.ppjwa.cn/gtkwgxbrls.html

find . -name "*.log" -type f
来源：http://hz.hysaishi.cn/gthzyjsxhk.html

[R44] 按修改时间查找
来源：http://hz.ehwqpu.com/gtgjuakbzw.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtcyjfepej.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtggroorha.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtlymkqxcc.html

[R46] 递归替换文件内容
来源：http://hz.chenlongwang.top/gtifdyatlu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtgikcicor.html

[R47] sed 单行替换
来源：http://hz.jinghuilouyu.cn/gtheoywqkb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guowangkeji.top/gteghinuub.html

[R48] awk 取指定列
来源：http://hz.dianchejie.cn/gtnspczcte.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtmpavcphr.html

[R49] awk 带条件
来源：http://hz.cdnleiting.top/gtjrsxryuq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtnvukvkir.html

[R50] awk 求和
来源：http://hz.yj20258888.top/gtftdeyisg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtriziibvc.html

[R51] 排序去重取前几
来源：http://hz.wangdashe.top/gtfuefngfk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pengpengdd.cyou/gtrfytawmd.html

[R52] 统计行数
来源：http://hz.gaohongyu789.top/gtctgustqm.html

wc -l a.txt
来源：http://hz.zhiwuduotai.top/gtsgcxkgko.html

[R53] 查看文件头与实时尾
来源：http://hz.birdmap.top/gtkucjewwz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj202588.top/gtxlohttgn.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtxjvuamry.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gtgovvcotw.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtdjazwoaz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.c1oappe.top/gtcyejnmlm.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gttqehtdxp.html

scp file user@host:/path/
来源：http://hz.zycfv.cn/gtdoglqspo.html

[R57] 远程执行命令
来源：http://hz.haohaochexian.top/gtnqyojwfg.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtbokscswb.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtpkhioxgt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aibaodan.cn/gtgutrtxfb.html

[R59] 发 POST JSON
来源：http://hz.haohaochexian.top/gtrntrszkv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xylfe.cn/gthjedcxqq.html

[R60] 只看 HTTP 状态码
来源：http://hz.tianlin.xyz/gtiuttgovn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtorxibrzk.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtkqnlknzp.html

df -h;  du -sh *
来源：http://hz.chenzaomai.com/gtuatiakqa.html

[R62] 找最占空间的文件
来源：http://hz.dianchejie.cn/gtzprklkok.html

du -ah . | sort -rh | head -10
来源：http://hz.bjfxy.top/gtpmnfafzm.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gttfgitbjd.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtllymmlln.html

[R64] 结束进程
来源：http://hz.shzxlz.cn/gtnlreeoai.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtxfvdizli.html

[R65] 查看端口占用
来源：http://hz.jinqigfzy.top/gttwxtzflb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jianghu66.top/gtejwblsvp.html

[R66] 定时任务
来源：http://hz.hfpthk.cn/gtpjfcezes.html

crontab -e;  crontab -l
来源：http://hz.tanke756.top/gtokghfhdq.html

[R67] 生成随机十六进制串
来源：http://hz.tian-w.cn/gtksfnbgcd.html

openssl rand -hex 16
来源：http://hz.guowangkeji.top/gtkefywngo.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtxhbqajjd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gogol.net.cn/gtbzclosrd.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtlterqvcz.html

head -c 16 /dev/urandom | base64
来源：http://hz.fengsongda.top/gtkfpwjrgi.html

[R70] 时间戳与互转
来源：http://hz.zhoulong.xyz/gtdtsllwwy.html

date +%s;  date -d @1700000000
来源：http://hz.zhixingplan.top/gtzsjgquji.html

[R71] 日期格式化
来源：http://hz.ywan-chungtsiang.top/gtsnpmnxpl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gtvqldngyg.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gttxfhoevv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gogol.net.cn/gtjyhqvbhh.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtcvlcgsfm.html

split -l 1000 big.log part_
来源：http://hz.c1oappe.top/gtopbzamyg.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtitcyudbs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ydjk.org.cn/gthgimcvwv.html

[R75] 导出环境变量
来源：http://hz.cashguo.top/gtfsazynbj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtphvzfecm.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gthglrmqia.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtbpsaklal.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtfzzqgdjj.html

read -rp "请输入: " ans
来源：http://hz.yueranfly.top/gtxuhpnrhi.html

[R78] 交互式菜单
来源：http://hz.xuetiantiany.cn/gthwkvcpai.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daria6918.cn/gtjyuubfnl.html

[R79] 解析命令行选项
来源：http://hz.yueranfly.top/gtwgbvsqiu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtffhdyvrw.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtxfncbeev.html

time ./run.sh
来源：http://hz.mhx1999.top/gttwsopzuw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfadlmaot.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtecpdgllh.html

================================================================================
来源：http://hz.nwbrower.top/gtrpcfwbsn.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtwxroghwh.html

#include <stdio.h>
来源：http://hz.vqdsnc.cn/gtmlzbkson.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tanke756.top/gtdktynpxi.html

[S02] C：变量与格式化输出
来源：http://hz.fzhhl.top/gtfcdplvhw.html

int a = 10; printf("%d\n", a);
来源：http://hz.hywenlv.cn/gtdrmnhofq.html

[S03] C：读入整数
来源：http://hz.gzhubu.top/gtwcicjumm.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gthrkchnsn.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtvkbkkwjv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gtqosxdkei.html

[S05] C：字符串长度
来源：http://hz.zhijiandao.cn/gtwozadhas.html

strlen(s)
来源：http://hz.9152youxi.cn/gtyhcsjptf.html

[S06] C：字符串比较
来源：http://hz.hongshengwenyu.top/gtrkvsvrvc.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtzerogugr.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gthlmwtucm.html


<!-- 参考信息 -->