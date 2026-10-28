代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtztkwpwqe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hammf.cn/gtwviiornp.html

[Q39] 自连接（查上下级）
来源：http://hz.jyoumei.cn/gtbgvdwioz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtxxkrymwr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtdetvoigo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gtynhpgvur.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hywenlv.cn/gtkqhxqndb.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtfahinekc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sufxvd.cn/gtdqtnxyon.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zdqjudy.top/gtlxziokjo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtdxlrzdas.html

[Q42] 连接条件附加过滤
来源：http://hz.yongpay.top/gtcadqxjmj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtvyquohun.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigufen.top/gtpwofoawp.html

[Q43] 标量子查询
来源：http://hz.gogol.net.cn/gtypkdweqx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtorqjkatl.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtlqfuieva.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtwqeqsads.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtnhxbtwvy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtryptmnek.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtchsivrax.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtbimdjvol.html

[Q47] 与平均值比较
来源：http://hz.zhaomingkeji.xyz/gtqurobpeh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jyoumei.cn/gtfxmkbgfb.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtilmusgvr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtzjrjabfj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhiwuduotai.top/gtmzgbivex.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtaiowpshr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tanke756.top/gtlgyhkftw.html

[Q50] 批量更新
来源：http://hz.daria6918.cn/gtbdqubxiz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.316326.xyz/gtjyvuwphr.html

[Q51] 用子查询更新
来源：http://hz.hnxiangtu.top/gtggssrtqa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sxryk.cn/gtcusefiwr.html

[Q52] 删除指定行
来源：http://hz.tanke756.top/gtmbuinlke.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtzegggnhp.html

[Q53] 按条件删除
来源：http://hz.zhongyouzk.top/gtcbxuyuay.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtpoxsgepb.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtyjdmxxrx.html

TRUNCATE TABLE logs;
来源：http://hz.yongpay.top/gtmmimfkkd.html

[Q55] 排名（并列占位）
来源：http://hz.gogol.net.cn/gtviceksyc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xylfe.cn/gtjyvgupgn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtuvsdqqfg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtglytudbd.html

[Q57] 行号
来源：http://hz.cqqwz.cn/gtumtknhgd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtrtbkxeqq.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtveheguuy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.feifeiyinyue.top/gtxbzkpofv.html

[Q59] 分组内累计
来源：http://hz.xingfuxueyuan.xyz/gtdelsbhle.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gtevqtciac.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gthcnllcmy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yvedp.cn/gtgnklwrjv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gaohongyu789.top/gtpezmohgd.html

[Q61] 移动平均
来源：http://hz.meibo888.top/gtjsfzvniy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtzqckjvfu.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtglydokre.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gticjnmwep.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtfoeturan.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zycfv.cn/gtcwnyqmia.html

[Q64] 提交事务
来源：http://hz.cheryme.top/gtpqbdvwdi.html

COMMIT;
来源：http://hz.redwolf501.top/gtzzvjywuu.html

[Q65] 回滚事务
来源：http://hz.shuidangran.top/gtfuzmgaju.html

ROLLBACK;
来源：http://hz.c1oappe.top/gtmgjultvf.html

[Q66] 行锁查询
来源：http://hz.yuanzhike.top/gtqrpopsul.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtsebxnyux.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtnyzedkww.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtfiegbrjw.html

[Q68] 保存点
来源：http://hz.zhongyouzk.top/gtcytxzcpd.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtqxzffupg.html

ROLLBACK TO sp1;
来源：http://hz.c1oappe.top/gtoxotjfdu.html

[Q69] 查看执行计划
来源：http://hz.cheryme.top/gtggvplckf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtjjioggvf.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gtvlthasyt.html

ANALYZE TABLE users;
来源：http://hz.tianlin.xyz/gtbrfepvlf.html

[Q71] 查看建表语句
来源：http://hz.zhiwuduotai.top/gtymzyqais.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenlongwang.top/gtaiebhqkw.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtwqxakdut.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtzfbcwhks.html

[Q73] 查看表状态
来源：http://hz.birdmap.top/gtblrdqrpe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtzpwointk.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtfofbfosh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gtsrwoumvx.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gtrxdcyayv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtyvstxymv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhijiandao.cn/gthzaaqzxf.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gtgadylmxd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtumtrholz.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtbyiaowir.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gttvwttelo.html

[Q78] 当前时间
来源：http://hz.ydjk.org.cn/gttcumoksl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtfyeyobdf.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gtwudxwgrc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.iojbl.cn/gtsnqytpqo.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gtxbmunjle.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gtludonlri.html

[Q81] 字符串替换
来源：http://hz.zycfv.cn/gtgmucxcsk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258.top/gtwohntzzq.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtilzdnvpm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtqiskhvwq.html

[Q83] 大小写转换
来源：http://hz.xziqi.cn/gtgxwwuvmy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guowangkeji.top/gtkdclyalz.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtmoqnopvv.html

SELECT TRIM(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtbxdmiomk.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtpplsdkut.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yangfankeji.com/gtfrigulvs.html

[Q86] 读取 JSON 字段
来源：http://hz.yueranfly.top/gtliyprjff.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yanxiufei.cn/gtivavhgny.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gttimjvtch.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangshuangyany.cn/gtfkkcqxdu.html

[Q88] 行转列（条件聚合）
来源：http://hz.nwbrower.top/gtqgkoomqx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangdashe.top/gtuktapqfs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yonumen.top/gtlqtdgcsh.html

[Q89] 判断表是否存在
来源：http://hz.hongshengwenyu.top/gtvfarjckq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tian-w.cn/gtmfzecrau.html

[Q90] 生成序号列
来源：http://hz.ybcxt.top/gtakyswdsf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258.top/gtviarsael.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwgrnkdbc.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtkokrcedl.html

================================================================================
来源：http://hz.jyoumei.cn/gtshltiuyh.html

[R01] shebang 与严格模式
来源：http://hz.snrcjt.cn/gtymqselog.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtycaiyhjc.html

set -euo pipefail
来源：http://hz.shangyingyoupin.top/gtdswylysx.html

[R02] 变量赋值与使用
来源：http://hz.yongpay.top/gtsydzjgoj.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtadwxrxxt.html

[R03] 只读变量
来源：http://hz.aibaodan.cn/gtzzwhukos.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtqfyqprax.html

[R04] 位置参数
来源：http://hz.cdnleiting.top/gtpaituwuf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtfcbvhype.html

[R05] 参数默认值
来源：http://hz.zhiwuduotai.top/gtvfrwesdo.html

name="${1:-default}"
来源：http://hz.cdnleiting.top/gtvozyobnb.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gthggchmpa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gogol.net.cn/gtovywfpee.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtddduikza.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jiagoushi.top/gtbnqxwmnb.html

[R08] 数值比较
来源：http://hz.guannengcc.top/gtlwpsnbmh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtgwvxftqw.html

[R09] 字符串比较
来源：http://hz.52xcode.cn/gttvtlmsct.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pengpengdd.cyou/gtejuznjbc.html

[R10] 正则匹配
来源：http://hz.jiagoushi.top/gtediisqjb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xinyue.icu/gtfjlzfzit.html

[R11] case 多分支
来源：http://hz.ydzc1.top/gtbbtbqpck.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtnozfvwkg.html

start) echo "启动" ;;
来源：http://hz.daria6918.cn/gtqaszjewj.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gtruvwifnh.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gtcldlgiru.html

esac
来源：http://hz.jyoumei.cn/gttuwtgnkn.html

[R12] for 遍历文件
来源：http://hz.sufxvd.cn/gtvbabdwys.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuetiantiany.cn/gtgoasjpxr.html

[R13] for 计数循环
来源：http://hz.sufxvd.cn/gtlkzdfvmj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtvqmajoss.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gtroxuysib.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtvllhgomw.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtuyzaiawl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtjivfpejv.html

[R16] until 等待条件
来源：http://hz.sweek.top/gthtklnimc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtxtgymuyt.html

[R17] 数组定义与取值
来源：http://hz.yongpay.top/gtceahrwfa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hysaishi.cn/gtspwdwccs.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gttlntgdwv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxinkj.top/gtvigqxjes.html

[R19] 数组长度
来源：http://hz.meibo888.top/gtecshfawz.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtdsonkawm.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtbjpsrqny.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtxmickphn.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtbpjfhayq.html

echo "${#s}"
来源：http://hz.c1oappe.top/gthfcizioo.html

[R22] 截取子串
来源：http://hz.quarkkingdee.top/gtraybwgxz.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtserbmrgk.html

[R23] 字符串替换
来源：http://hz.kuanghao11.cn/gtsgjcovap.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtxnbmuutg.html

[R24] 大小写转换
来源：http://hz.fengsongda.top/gtpibqnvga.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtimhkbgvo.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtytvvrmjc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtinzkelbc.html

[R26] 命令替换
来源：http://hz.andypj.xyz/gtkcbjrkix.html

now=$(date +%F); echo "$now"
来源：http://hz.fengsongda.top/gtxirbghyz.html

[R27] 算术展开
来源：http://hz.sweek.top/gtfhgejomv.html

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gtoxjqcjlz.html

[R28] 浮点运算
来源：http://hz.tianlin.xyz/gtcmlohvsk.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangshuangyany.cn/gttjoogrhn.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gttaslrskk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtsowjmvxe.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtevzhuooz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.snrcjt.cn/gtyvlbfxhz.html

[R31] 局部变量
来源：http://hz.havefunace.top/gtknnorqvg.html

f() { local x=1; echo "$x"; }
来源：http://hz.iojbl.cn/gtbfnyldku.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gtmcoibdxk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guowangkeji.top/gtzkiuhxxe.html

[R33] 捕获错误并提示行号
来源：http://hz.chenjidiqi.icu/gtdptawfkt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtvhtqhrgi.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtgoerueuq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtextrvytc.html

[R35] 后台执行并等待
来源：http://hz.ehwqpu.com/gttjwongaq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gttmniqsne.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtsuvmncxz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.wangdashe.top/gtxzmkiyea.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtaxskncfm.html

files=$(ls -1)
来源：http://hz.hywenlv.cn/gtdnjrkist.html

[R38] 管道串联
来源：http://hz.yuxming.cn/gtswtphxyy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.snrcjt.cn/gtfbvsjxys.html

[R39] 重定向标准输出与错误
来源：http://hz.ehwqpu.com/gtluqgyfus.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gtmwtbphfd.html

[R40] 追加写日志
来源：http://hz.svipenyu.cn/gtprxyldrw.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtpkimlqqn.html

[R41] 丢弃输出
来源：http://hz.redwolf501.top/gtwloskzwi.html

cmd >/dev/null 2>&1
来源：http://hz.hammf.cn/gtayncffik.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtbszlptbx.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtpetgiuac.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gthmoecmnw.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gtvajbiazn.html

[R44] 按修改时间查找
来源：http://hz.kuanghao11.cn/gtwguexoiq.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gticzucmdb.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtjnzpujbe.html

find . -name "*.tmp" -delete
来源：http://hz.yonumen.top/gtqizmswif.html

[R46] 递归替换文件内容
来源：http://hz.jyoumei.cn/gtmliytstc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.andypj.xyz/gtadhxxjwt.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtiocsrvwx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tanke756.top/gtkimffqez.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtzvjtrxxd.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtgrcfcuyx.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtbrnkmvqh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtaimtbaym.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtrpfdeaov.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shangyingyoupin.top/gtetunqywl.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtiwjfodjz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aibaodan.cn/gtfkpajmie.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gttjdsphhz.html

wc -l a.txt
来源：http://hz.meibo888.top/gtsazuokus.html

[R53] 查看文件头与实时尾
来源：http://hz.jianghu66.top/gtpuwlckyk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangtech.top/gthvkuzntr.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtxsdfatfo.html

diff a.txt b.txt
来源：http://hz.shanyushiyangkeji.top/gtnzzbapxx.html

[R55] 压缩与解压
来源：http://hz.tianlin.xyz/gtuadlutzx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tian-w.cn/gtadlgfopk.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtmvwbgmyc.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtzwlubxwg.html

[R57] 远程执行命令
来源：http://hz.cdnleiting.top/gtrnrajdlp.html

ssh user@host 'uptime'
来源：http://hz.jqgfzy.top/gtatalspoe.html

[R58] 下载文件
来源：http://hz.ivvv.top/gtmtkdbbxh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangkeji.top/gtdsmpyfqj.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtszlqboey.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yonumen.top/gtjoepisvu.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtrkjxzgsh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xylfe.cn/gtmgwacuhh.html

[R61] 磁盘占用
来源：http://hz.iojbl.cn/gtcvmtvdrh.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gtebpjgcmw.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtvqulzhxu.html

du -ah . | sort -rh | head -10
来源：http://hz.sufxvd.cn/gtponpigsq.html

[R63] 内存与进程
来源：http://hz.jyoumei.cn/gtxnesrjjs.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtxjcpnlxp.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gtjvhjxddb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.316326.xyz/gtzjyahgxg.html

[R65] 查看端口占用
来源：http://hz.fengsongda.top/gtgbxiwpzu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtgzgzizru.html

[R66] 定时任务
来源：http://hz.sufxvd.cn/gtehlyyiwp.html

crontab -e;  crontab -l
来源：http://hz.guannengcc.top/gtiimpjplg.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gttsryjkvg.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtaeuazwae.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtwnkkxaxm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cashguo.top/gtlqdzjpfc.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtkqkiqnqf.html

head -c 16 /dev/urandom | base64
来源：http://hz.xziqi.cn/gtwurznkmm.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtwphaqbdc.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtkzgcnuip.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtucerihty.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hysaishi.cn/gtwejzjeuv.html

[R72] 等待端口就绪
来源：http://hz.snrcjt.cn/gtaqejiywz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtdrmdylcj.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gteunuikwx.html

split -l 1000 big.log part_
来源：http://hz.kuanghao11.cn/gtqoccehox.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtdmkoqsgk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tian-w.cn/gtxrwsutfy.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtfrudnjtf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigfzy.top/gtrwfxcmgh.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtretwdjnn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtvioxyqnf.html

[R77] 读取用户输入
来源：http://hz.smart0.xyz/gtcplelshf.html

read -rp "请输入: " ans
来源：http://hz.52xcode.cn/gtvvswganl.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtpghfkjcd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gtnaqhqrfc.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gttomvniqq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ppjwa.cn/gtfyzgtgzi.html

[R80] 查看脚本执行耗时
来源：http://hz.aizwys.cn/gtfzdazvgh.html

time ./run.sh
来源：http://hz.tanke756.top/gtbzefltrn.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttedrqkvv.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtkzejjqzr.html

================================================================================
来源：http://hz.yangfankeji.com/gtywdcqucu.html

[S01] C：Hello World
来源：http://hz.ivvv.top/gtvkdvqjpl.html

#include <stdio.h>
来源：http://hz.sufxvd.cn/gtwcfbdupv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cheryme.top/gtoqupihtw.html

[S02] C：变量与格式化输出
来源：http://hz.wangshuangyany.cn/gthnxaydeq.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhengqikj.top/gtouwwxhie.html

[S03] C：读入整数
来源：http://hz.gaohongyu789.top/gtipzzeovm.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtvvrxhaqu.html

[S04] C：字符串复制
来源：http://hz.tianlin.xyz/gtkgixlfha.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtjrceqgab.html

[S05] C：字符串长度
来源：http://hz.zycfv.cn/gtridtkael.html

strlen(s)
来源：http://hz.cheryme.top/gtvhycucaq.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gthxyzdbss.html

strcmp(a, b) == 0
来源：http://hz.52xcode.cn/gtgosapjqa.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtcxtwzudo.html


<!-- 参考信息 -->