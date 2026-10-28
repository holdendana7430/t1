代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtmiookwaa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fzhhl.top/gtzjsmjskf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtpekzaglg.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtqicmwamd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.9152youxi.cn/gtcmvjjuip.html

JOIN users u ON u.id = o.user_id
来源：http://hz.svipenyu.cn/gtaqapwlgo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pycfn.com/gtyqezhfvn.html

[Q42] 连接条件附加过滤
来源：http://hz.ybcxt.top/gtxmakoplp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shzxlz.cn/gtvwzlurmk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtkrnofwzm.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gtxrwldehy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gtawjmapcq.html

[Q44] IN 子查询
来源：http://hz.chenzaomai.com/gttsktjusy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gtndodmokj.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gtunuykufb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtathqqhmp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgufenzy.top/gtgkwvqfji.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtcspxormv.html

[Q47] 与平均值比较
来源：http://hz.daria6918.cn/gtwravzppb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gttvgiizvp.html

[Q48] CTE 公用表表达式
来源：http://hz.kuanghao11.cn/gtueufnlhn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.dashuyun.cn/gtsufjqwym.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtywsgqpjh.html

[Q49] 更新单行
来源：http://hz.snrcjt.cn/gtewisvzdu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtmmkleyvk.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gtqlycmrlj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yuxming.cn/gtrsscmzzu.html

[Q51] 用子查询更新
来源：http://hz.yangfankeji.com/gtpffhdinr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jlsjyb.cn/gtzfdbcnui.html

[Q52] 删除指定行
来源：http://hz.xingfuxueyuan.xyz/gtwfewmlji.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtwgpzkfkn.html

[Q53] 按条件删除
来源：http://hz.bjfxy.top/gtfqdxcopy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sufxvd.cn/gtcqbaqdpj.html

[Q54] 清空表
来源：http://hz.zhongyouzk.top/gtsezyuhdx.html

TRUNCATE TABLE logs;
来源：http://hz.jyoumei.cn/gtfbllazby.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtcgrvlorz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.smart0.xyz/gtbmtaqloy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xingfuxueyuan.xyz/gtihocbiti.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtpjgmwnbt.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtyyyyxbdg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gtzghubtyg.html

[Q58] 累计求和
来源：http://hz.sufxvd.cn/gtwkgpztcg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj202588.top/gtjjhdzeai.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtzfxtdpkt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yongpay.top/gthrfznwij.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gttywpfqre.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ivvv.top/gtnfuktxlh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258.top/gtuioxkegx.html

[Q61] 移动平均
来源：http://hz.jqgufenzy.top/gtffynyyjp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.havefunace.top/gtoyobymmi.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gttgjipnnf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtojeaitdg.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtpshuraoy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dashuyun.cn/gtxxpertsp.html

[Q64] 提交事务
来源：http://hz.havefunace.top/gthzkhhyas.html

COMMIT;
来源：http://hz.jinqigufen.top/gtlfmkqfuc.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtwtkcrpij.html

ROLLBACK;
来源：http://hz.yj20258888.top/gtqtqyarfg.html

[Q66] 行锁查询
来源：http://hz.snrcjt.cn/gtrwuxcrry.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtpzhponih.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtmgeppbip.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangdashe.top/gtuzanqngh.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gtiuevmtpv.html

SAVEPOINT sp1;
来源：http://hz.kuanghao11.cn/gtnrguduzb.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtfboziaiu.html

[Q69] 查看执行计划
来源：http://hz.sysykeji.top/gtlhbhjoup.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ywan-chungtsiang.top/gtadbqinbb.html

[Q70] 更新统计信息
来源：http://hz.ehwqpu.com/gtqvufslyv.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtjipjpbdc.html

[Q71] 查看建表语句
来源：http://hz.nwbrower.top/gthmvapgmf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtyieppzvj.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gttciyaihz.html

SHOW INDEX FROM users;
来源：http://hz.sxryk.cn/gtdsvrqwfv.html

[Q73] 查看表状态
来源：http://hz.zhongyouzk.top/gtwygraueg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gteicanlsu.html

[Q74] 强制使用索引
来源：http://hz.cdnleiting.top/gtarcmmhnt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sweek.top/gtcetnezmn.html

[Q75] 日期格式化
来源：http://hz.ppjwa.cn/gtrypgoozz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtfrwquaou.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gtzshosyzt.html

[Q76] 按天统计
来源：http://hz.guowangkeji.top/gtfypymlry.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.redwolf501.top/gthmmuntsd.html

[Q77] 时间加减
来源：http://hz.vqdsnc.cn/gttqbuqtds.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangkeji.top/gtjzesbdfu.html

[Q78] 当前时间
来源：http://hz.hysaishi.cn/gtcgppielw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nwbrower.top/gtqvjmucqh.html

[Q79] 字符串拼接
来源：http://hz.sweek.top/gtgdjjygpp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtdtyrybvy.html

[Q80] 字符串截取
来源：http://hz.0kj1m.cn/gtydwiacna.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gtlgsxlqdh.html

[Q81] 字符串替换
来源：http://hz.zhongyouzk.top/gtwmaaxkox.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daria6918.cn/gtrsstiery.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gteseayhka.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.vqdsnc.cn/gtcuiubgnf.html

[Q83] 大小写转换
来源：http://hz.gaohongyu789.top/gttxlkqmfp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtxbqzycmo.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gtsqrxhtmh.html

SELECT TRIM(name) FROM users;
来源：http://hz.snrcjt.cn/gtdznevlpy.html

[Q85] 数值取整
来源：http://hz.wangshuangyany.cn/gtbnxhxhmy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yonumen.top/gtirzddgay.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258888.top/gtiilrzpse.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sxryk.cn/gtxejymulv.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtoxbbszzt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.snrcjt.cn/gtedgufhrj.html

[Q88] 行转列（条件聚合）
来源：http://hz.tianlin.xyz/gtbgmvljxr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtggrzixqm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hywenlv.cn/gtsabojrwo.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtukgnkyyk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtfrevrmqq.html

[Q90] 生成序号列
来源：http://hz.wangdashe.top/gtgrhjwhom.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinghuilouyu.cn/gtooeselcc.html

================================================================================
来源：http://hz.yvedp.cn/gtukkqlmsy.html

R. Bash 专题
来源：http://hz.pycfn.com/gthsleqtin.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjzlrcbyz.html

[R01] shebang 与严格模式
来源：http://hz.yj20258.top/gtagsrinmh.html

#!/usr/bin/env bash
来源：http://hz.zhiwuduotai.top/gtljlovlhw.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtabujeblw.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtbflbqwzz.html

name="Tom"; echo "$name"
来源：http://hz.daria6918.cn/gtelnkvyxi.html

[R03] 只读变量
来源：http://hz.hysaishi.cn/gtdpjykffb.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtiiekuyei.html

[R04] 位置参数
来源：http://hz.aibaodan.cn/gtrlqvqekb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gtzwvkyest.html

[R05] 参数默认值
来源：http://hz.nanxuanxn.top/gtnzjtaoti.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtayobxkfc.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gtngytafem.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuanzhike.top/gtxqyjyfmj.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gtjdniohhn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.andypj.xyz/gtxzrbvkam.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gtygmagsxm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gtparowrzr.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtaxybgikp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtlgbylcxx.html

[R10] 正则匹配
来源：http://hz.sufxvd.cn/gtlirhhrta.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gogol.net.cn/gtimrhahsc.html

[R11] case 多分支
来源：http://hz.zhiwuduotai.top/gtlwccrsme.html

case "$1" in
来源：http://hz.hywenlv.cn/gtvpysvxwp.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gtgceugugh.html

stop)  echo "停止" ;;
来源：http://hz.zdqjudy.top/gtxthubpar.html

*)     echo "未知命令" ;;
来源：http://hz.ppjwa.cn/gtqjoslwmb.html

esac
来源：http://hz.fzhhl.top/gtllossevn.html

[R12] for 遍历文件
来源：http://hz.cheryme.top/gtbembyjcc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shzxlz.cn/gteejfyjwo.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtllqxfcxh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtdnkefxtg.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtbyzygshb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yangfankeji.com/gtjfkjmivj.html

[R15] while 逐行读文件
来源：http://hz.316326.xyz/gtpviehdmh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtulntsbsx.html

[R16] until 等待条件
来源：http://hz.kuanghao11.cn/gtqgikygiv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yangfankeji.com/gtwwatgcdc.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtjyehzdxa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.iojbl.cn/gtnsidonlc.html

[R18] 遍历数组
来源：http://hz.wangshuangyany.cn/gtbqrhhcpw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.smart0.xyz/gtdyukhilq.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtvvrhntfz.html

echo "${#arr[@]}"
来源：http://hz.daria6918.cn/gtfbtyelfz.html

[R20] 关联数组（字典）
来源：http://hz.chenlongwang.top/gtstiqyksc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinghuilouyu.cn/gtqtqwlndt.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtmerynerb.html

echo "${#s}"
来源：http://hz.yj20258888.top/gtnqfsblnw.html

[R22] 截取子串
来源：http://hz.xinyue.icu/gtysoqsbrd.html

echo "${s:0:5}"
来源：http://hz.snrcjt.cn/gtjtsqckfi.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtbusqwrqg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtmapvczhi.html

[R24] 大小写转换
来源：http://hz.bjfxy.top/gtbfyljaqh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gtvwvdxggw.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtpoxhlvik.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hywenlv.cn/gtgkkozjoy.html

[R26] 命令替换
来源：http://hz.cucudq.cn/gtyogcukkk.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gthcsaywxa.html

[R27] 算术展开
来源：http://hz.hywenlv.cn/gtcjwudwrw.html

echo $((1 + 2 * 3))
来源：http://hz.yj202588.top/gthjosxkox.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtnrabnczn.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenlongwang.top/gtlgtvctec.html

[R29] 定义函数
来源：http://hz.zhengqikj.top/gtdtifyqkl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtgrhphsct.html

[R30] 函数返回状态码
来源：http://hz.daria6918.cn/gtxuzaaaae.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guowangkeji.top/gtidsvbolj.html

[R31] 局部变量
来源：http://hz.meibo888.top/gtroztxbae.html

f() { local x=1; echo "$x"; }
来源：http://hz.vqdsnc.cn/gtqzsthmrb.html

[R32] 参数个数校验
来源：http://hz.daxiang520.top/gtjgbgkokx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.aibaodan.cn/gtmosstsza.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gtsbjeepwm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtuznzymnh.html

[R34] 退出时清理
来源：http://hz.xuanzx.com/gtfmlqkfbm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtsevnhlbv.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gthnekptqx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gtoxawcqie.html

[R36] 并发执行多个任务
来源：http://hz.redwolf501.top/gtawohcikt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cdnleiting.top/gtkceehxkl.html

[R37] 把输出赋给变量
来源：http://hz.yongpay.top/gtsxgiurts.html

files=$(ls -1)
来源：http://hz.wangdashe.top/gtqkkcyxbn.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtuhmhtvyr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtjzpeommk.html

[R39] 重定向标准输出与错误
来源：http://hz.c1oappe.top/gtzujnnzwk.html

cmd > out.log 2>&1
来源：http://hz.zhixingplan.top/gtwunrscnl.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtoxfzypmy.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtezivnsvb.html

[R41] 丢弃输出
来源：http://hz.svipenyu.cn/gtokkyogqm.html

cmd >/dev/null 2>&1
来源：http://hz.jinyuanbaomall.cn/gtgxqfmqlb.html

[R42] 输入重定向
来源：http://hz.zhoulong.xyz/gtwvckpney.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtpktavnwx.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtvzpzfssc.html

find . -name "*.log" -type f
来源：http://hz.sweek.top/gtsbjvkqah.html

[R44] 按修改时间查找
来源：http://hz.ppjwa.cn/gtiogzjtdb.html

find . -mtime -7 -type f
来源：http://hz.zhaomingkeji.xyz/gtlracbyoi.html

[R45] 批量删除
来源：http://hz.shanyushiyangkeji.top/gtexacwugi.html

find . -name "*.tmp" -delete
来源：http://hz.sufxvd.cn/gtaodinfvr.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtzrystvxf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnqzz.top/gtlcifwgbj.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gteukmzjud.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.quarkkingdee.top/gttamdnykc.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtxtudvshc.html

awk '{print $1, $3}' a.txt
来源：http://hz.redwolf501.top/gtnlmdjhve.html

[R49] awk 带条件
来源：http://hz.jinqigufen.top/gtmeklrqcb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtvrkdnaib.html

[R50] awk 求和
来源：http://hz.yj20258.top/gtfjqhtycx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gthssrpfhj.html

[R51] 排序去重取前几
来源：http://hz.kuanghao11.cn/gtplezjbpz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhixingplan.top/gtnpytmcej.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtoledtibs.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtivtrftom.html

[R53] 查看文件头与实时尾
来源：http://hz.kuanghao11.cn/gtzyvaklzo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zycfv.cn/gtesyozpzx.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtwnuvsexr.html

diff a.txt b.txt
来源：http://hz.iojbl.cn/gtbgrxgrwa.html

[R55] 压缩与解压
来源：http://hz.hywenlv.cn/gteqqzgbdp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtiipajbpy.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtwikbwuxz.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtfwfuaakh.html

[R57] 远程执行命令
来源：http://hz.vqdsnc.cn/gtyeqgwgwf.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gtnsawhpqj.html

[R58] 下载文件
来源：http://hz.cucudq.cn/gtuvyvihot.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangkeji.top/gtmtfgtgce.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtjvibvgtk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.guannengcc.top/gtpmzaknio.html

[R60] 只看 HTTP 状态码
来源：http://hz.yueranfly.top/gttiekmbof.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yongpay.top/gtwtuesuyq.html

[R61] 磁盘占用
来源：http://hz.ppjwa.cn/gtztlhifis.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gthjxgpomm.html

[R62] 找最占空间的文件
来源：http://hz.jinyuanbaomall.cn/gtbisxfwev.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtkscvwccp.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtmlevdklc.html

free -h;  ps aux | grep nginx
来源：http://hz.nwbrower.top/gtidvnmkbp.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtubeexxtf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hywenlv.cn/gtyhpctymk.html

[R65] 查看端口占用
来源：http://hz.yj20258.top/gtpydrzank.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnxiangtu.top/gtviptbjrq.html

[R66] 定时任务
来源：http://hz.xziqi.cn/gtjyqvtzdq.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtoblbrcbj.html

[R67] 生成随机十六进制串
来源：http://hz.sweek.top/gtcaexetlu.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtdefbvnjp.html

[R68] 计算文件校验值
来源：http://hz.jinqigfzy.top/gtazuphwgi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtijbnsblk.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtihntutaw.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gtvnanayhw.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtixmktgcu.html

date +%s;  date -d @1700000000
来源：http://hz.ivvv.top/gttdlqkewn.html

[R71] 日期格式化
来源：http://hz.smart0.xyz/gtpvlfdnsf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aibaodan.cn/gtexuywqss.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtecaklhht.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gtfixiuwei.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gtmcqjywrt.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtvprlelxi.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gtyjgvdwtl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigufen.top/gtggtojnhk.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtopwwksuw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cashguo.top/gtyvhvecvm.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtskjgmmtz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fzhhl.top/gtmxlghkfb.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtnsqcrlco.html

read -rp "请输入: " ans
来源：http://hz.cqqwz.cn/gtlfymtmns.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtiutaouvv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhijiandao.cn/gtxnwdzqki.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtuubeswcg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.kuanghao11.cn/gtcfemewzj.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gteairwjwn.html

time ./run.sh
来源：http://hz.xziqi.cn/gtwtgeqkoi.html

================================================================================
来源：http://hz.gogol.net.cn/gtlhrvefoc.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtdnitnfpi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcgpbzkfc.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtfghgrzbb.html

#include <stdio.h>
来源：http://hz.sufxvd.cn/gtpfznwklz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgufenzy.top/gtqlhhniey.html

[S02] C：变量与格式化输出
来源：http://hz.pycfn.com/gtarcdyhht.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhoulong.xyz/gtdckqplpx.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gtxlpvbmyy.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtyvuiegpl.html

[S04] C：字符串复制
来源：http://hz.aizwys.cn/gtznqtvegy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gtzllqvutb.html

[S05] C：字符串长度
来源：http://hz.xuetiantiany.cn/gtlvqeucoh.html

strlen(s)
来源：http://hz.chenzaomai.com/gtcmwdpytc.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtldlgmiqr.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtszptaduh.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gtwexyicze.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangtech.top/gthsqysltd.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258.top/gtdyxnspqv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydzc1.top/gtsertekxb.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtdzdgzgag.html


<!-- 参考信息 -->