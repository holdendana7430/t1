代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.andypj.xyz/gtkijrqdgs.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtiiknhkla.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.dianchejie.cn/gtwaongjii.html

[Q51] 用子查询更新
来源：http://hz.aibaodan.cn/gtvgjbifgk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydjk.org.cn/gtspjllfqp.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gtzrohzyio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xinyue.icu/gtdluowtje.html

[Q53] 按条件删除
来源：http://hz.gaohongyu789.top/gtezkvocgh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sxryk.cn/gtgstrntmb.html

[Q54] 清空表
来源：http://hz.jinghuilouyu.cn/gtgdnxkynm.html

TRUNCATE TABLE logs;
来源：http://hz.yongpay.top/gtzasqduhr.html

[Q55] 排名（并列占位）
来源：http://hz.jyoumei.cn/gtluwblvey.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtoryjhvbd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.iojbl.cn/gtkfdspmcw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtncceeflj.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtpirzqilo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigufen.top/gtdiutqlum.html

[Q58] 累计求和
来源：http://hz.shanyushiyangtech.top/gtioskoaoo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.mhx1999.top/gtzfrklqnd.html

[Q59] 分组内累计
来源：http://hz.wangshuangyany.cn/gtzxlbczky.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ydjk.org.cn/gtdsjxaaew.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtiaieuewk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangkeji.top/gtkuybuyzu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtmtlymfls.html

[Q61] 移动平均
来源：http://hz.zdqjudy.top/gtmmlwsnxr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtzaubwxyq.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtqxpmnlpr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtlhyxtwrd.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gtuwducebx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gtzizxynot.html

[Q64] 提交事务
来源：http://hz.cashguo.top/gtfqihfojd.html

COMMIT;
来源：http://hz.yonumen.top/gtdcckvuim.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gttkfyiwsd.html

ROLLBACK;
来源：http://hz.dashuyun.cn/gtczxsxpqa.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gtpvjnhlgo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.meibo888.top/gtqajlyumk.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtvklykyox.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtejkeqjos.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gtucpqmyoj.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtbnyyandw.html

ROLLBACK TO sp1;
来源：http://hz.chenjidiqi.icu/gtzgrxjetu.html

[Q69] 查看执行计划
来源：http://hz.jinyuanbaomall.cn/gtisdviooh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258888.top/gtvhkeyone.html

[Q70] 更新统计信息
来源：http://hz.gogol.net.cn/gtvkhvtmud.html

ANALYZE TABLE users;
来源：http://hz.cdnleiting.top/gtkmduoxtg.html

[Q71] 查看建表语句
来源：http://hz.daxiang520.top/gtltpuwcjb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhongyouzk.top/gtrpurcaud.html

[Q72] 查看索引
来源：http://hz.ppjwa.cn/gtqzmqbsak.html

SHOW INDEX FROM users;
来源：http://hz.jinyuanbaomall.cn/gtudjclysh.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtmrcpbldt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.kuanghao11.cn/gtzjkjqfhq.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gtgpmfdnnj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gttxianmud.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gthfuvvqpf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jyoumei.cn/gtatjjiqga.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shangyingyoupin.top/gthmcafvxa.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtttkthuqe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.havefunace.top/gtizsqymbi.html

[Q77] 时间加减
来源：http://hz.ybcxt.top/gtoffaylvy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtmunaekrm.html

[Q78] 当前时间
来源：http://hz.hnqzz.top/gtmjpzoykg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinyuanbaomall.cn/gtqwmwxytx.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtorjmtuvk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gotoacloud.top/gtcuxqhlrv.html

[Q80] 字符串截取
来源：http://hz.jqgfzy.top/gtoympvzln.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tianlin.xyz/gthkuvntac.html

[Q81] 字符串替换
来源：http://hz.hammf.cn/gtecbfqpdw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtlorjzftp.html

[Q82] 字符长度与字节长度
来源：http://hz.chenzaomai.com/gtzpxhxllp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gaohongyu789.top/gtxepkhenp.html

[Q83] 大小写转换
来源：http://hz.fengsongda.top/gteppegjnm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuanzx.com/gtrdvosoqc.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gtctiswhtl.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydzc1.top/gtwztdfxjt.html

[Q85] 数值取整
来源：http://hz.andypj.xyz/gtuumxmxhm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.quarkkingdee.top/gtrabqiapx.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtrcwodwxj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sweek.top/gtogucsrhr.html

[Q87] JSON 字段做条件
来源：http://hz.zhiwuduotai.top/gtegypifqo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aibaodan.cn/gtijizdtft.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtlaxlyepo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gteeuxrkrt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hfpthk.cn/gtoapuqpwo.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtyhozwfob.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fzhhl.top/gtsmzdgkbs.html

[Q90] 生成序号列
来源：http://hz.hfpthk.cn/gtrdstjkvl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zdqjudy.top/gtwbrdcslm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxpewluks.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gtmtcvnlie.html

================================================================================
来源：http://hz.0kj1m.cn/gtdzvlhiva.html

[R01] shebang 与严格模式
来源：http://hz.yueranfly.top/gtswtoptdh.html

#!/usr/bin/env bash
来源：http://hz.vqdsnc.cn/gtxprnqvim.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gtaqndplyd.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtphbthmud.html

name="Tom"; echo "$name"
来源：http://hz.9152youxi.cn/gtjeampayj.html

[R03] 只读变量
来源：http://hz.zhixingplan.top/gtpwejkmct.html

readonly PI=3.14
来源：http://hz.gotoacloud.top/gtznkcnzsw.html

[R04] 位置参数
来源：http://hz.jqgfzy.top/gtzcuxhajk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cdnleiting.top/gtjganfkje.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtmhnzicbz.html

name="${1:-default}"
来源：http://hz.ybcxt.top/gtydmlcknn.html

[R06] 判断命令是否存在
来源：http://hz.daxiang520.top/gtadcennbk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yonumen.top/gtpgzenzsi.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtzlcxaupw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnxiangtu.top/gtfjdtwrhj.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtiamdpstp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxinkj.top/gtqoisstcq.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtfgumhsxf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtqinuvyhm.html

[R10] 正则匹配
来源：http://hz.smart0.xyz/gtocavvfnq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtqlnpicdz.html

[R11] case 多分支
来源：http://hz.shanyushiyangtech.top/gtadgmkskl.html

case "$1" in
来源：http://hz.0kj1m.cn/gtlpiyldov.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtvvramyns.html

stop)  echo "停止" ;;
来源：http://hz.zhijiandao.cn/gtufhxmwej.html

*)     echo "未知命令" ;;
来源：http://hz.tanke756.top/gthewdaugi.html

esac
来源：http://hz.guowangkeji.top/gtazazkkja.html

[R12] for 遍历文件
来源：http://hz.fengsongda.top/gtiexlvaty.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtmzhqqasn.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtwgqzjoka.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtsbcztxjt.html

[R14] C 风格 for
来源：http://hz.yangfankeji.com/gtemithjji.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtyuhurygm.html

[R15] while 逐行读文件
来源：http://hz.jinghuilouyu.cn/gteioknrvn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgfzy.top/gtugumjdmi.html

[R16] until 等待条件
来源：http://hz.bjfxy.top/gtmutybqua.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtlnktjgus.html

[R17] 数组定义与取值
来源：http://hz.andypj.xyz/gtohilclmx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtnzkojuaw.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtruyjtxjl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtjbavucay.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gtkascmhqp.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gtgmialjtp.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gtjplynrbj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtzfrtrnar.html

[R21] 字符串长度
来源：http://hz.shanyushiyangtech.top/gtojdqxtpx.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtveqpjhxt.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtkfdvbckg.html

echo "${s:0:5}"
来源：http://hz.ehwqpu.com/gtplxxvyoi.html

[R23] 字符串替换
来源：http://hz.chenzaomai.com/gtjpchckfe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtoweflwqv.html

[R24] 大小写转换
来源：http://hz.gotoacloud.top/gtxdnyeoos.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pycfn.com/gtjvdebzdv.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gtqlvdfpeo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigfzy.top/gthbvbxbau.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtcxuvjlez.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gthhmfuedx.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtkxxvegzb.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258.top/gtsnsncqyp.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gtblehozaz.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxuanxn.top/gtdadvpgig.html

[R29] 定义函数
来源：http://hz.shuidangran.top/gtednegchz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtgplpkdes.html

[R30] 函数返回状态码
来源：http://hz.xingfuxueyuan.xyz/gtcbemryhy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gtsgrfaltd.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gtzmfpqldy.html

f() { local x=1; echo "$x"; }
来源：http://hz.cdnleiting.top/gtmhxssokf.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtousbsgjv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cashguo.top/gticjzcbrp.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtdxogjjia.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sysykeji.top/gtagqgefwh.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gttvqnbtyh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtoiucmhtn.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtfpyevmib.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gttpthcljf.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gtohvjbrds.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cdnleiting.top/gthvqglffx.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtfjmezlgl.html

files=$(ls -1)
来源：http://hz.guowangkeji.top/gtvaljgomn.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gttojervvq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhongyouzk.top/gtiaoqzrcx.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtwoqshcxm.html

cmd > out.log 2>&1
来源：http://hz.yanxiufei.cn/gtuaoxgoch.html

[R40] 追加写日志
来源：http://hz.yangfankeji.com/gtjqofcgdt.html

echo "log" >> out.log
来源：http://hz.aibaodan.cn/gtwuejmtga.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtuazhyayq.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtupzzvmva.html

[R42] 输入重定向
来源：http://hz.bjfxy.top/gtrigkzkpc.html

wc -l < a.txt
来源：http://hz.sufxvd.cn/gtfhedmbov.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtrfrdkeah.html

find . -name "*.log" -type f
来源：http://hz.cucudq.cn/gtxxccadex.html

[R44] 按修改时间查找
来源：http://hz.c1oappe.top/gtoqegiasj.html

find . -mtime -7 -type f
来源：http://hz.0kj1m.cn/gtvulhllpl.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtihizkikg.html

find . -name "*.tmp" -delete
来源：http://hz.gotoacloud.top/gtxlfgcywv.html

[R46] 递归替换文件内容
来源：http://hz.jyoumei.cn/gtuakgbatq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gttfjrvhqo.html

[R47] sed 单行替换
来源：http://hz.gzhubu.top/gtyxtdpmld.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtvayulvdq.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtrqeqnwih.html

awk '{print $1, $3}' a.txt
来源：http://hz.snrcjt.cn/gtrtjbkwtl.html

[R49] awk 带条件
来源：http://hz.shanyushiyangkeji.top/gtmhuzgomp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.mhx1999.top/gtmekzzchk.html

[R50] awk 求和
来源：http://hz.ydjk.org.cn/gtyqjsczpi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinghuilouyu.cn/gtanrcvasa.html

[R51] 排序去重取前几
来源：http://hz.nanxinkj.top/gtccggbxbi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.smart0.xyz/gtwknnxxna.html

[R52] 统计行数
来源：http://hz.redwolf501.top/gtvzpvaxmw.html

wc -l a.txt
来源：http://hz.zhongyouzk.top/gteyelyngt.html

[R53] 查看文件头与实时尾
来源：http://hz.redwolf501.top/gterztcgcz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.mhx1999.top/gttithtmfd.html

[R54] 比较两个文件
来源：http://hz.hongshengwenyu.top/gtbhypoans.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gtouzxumfn.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtbhurpkza.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.iojbl.cn/gtmahjimsx.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtyehsvwrx.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gtjhnywrsq.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtdqqkyrbs.html

ssh user@host 'uptime'
来源：http://hz.cashguo.top/gtbexuidcr.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gtpzitdotx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydjk.org.cn/gtiphwmyld.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtzntiymvs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtsfvskluy.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtjqgbbdac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtiyxaebti.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtznqsmatz.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gtqazzmofd.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gtdhnockau.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtslqfhujs.html

[R63] 内存与进程
来源：http://hz.jqgfzy.top/gtgvpqyieq.html

free -h;  ps aux | grep nginx
来源：http://hz.ydjk.org.cn/gtafldgpdl.html

[R64] 结束进程
来源：http://hz.ywan-chungtsiang.top/gtncwhiyng.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtlifsuzml.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangtech.top/gtphmbonlh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtqzfqidcj.html

[R66] 定时任务
来源：http://hz.wangdashe.top/gtwwrlxgku.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gtjezocoqv.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtnqqeuher.html

openssl rand -hex 16
来源：http://hz.zhengqikj.top/gtwhriuhrm.html

[R68] 计算文件校验值
来源：http://hz.bjfxy.top/gtzxfrrsyp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hammf.cn/gtemhbbppl.html

[R69] 生成随机密码
来源：http://hz.shuidangran.top/gterodlqfl.html

head -c 16 /dev/urandom | base64
来源：http://hz.xingfuxueyuan.xyz/gtwjntuzwj.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gtililhfth.html

date +%s;  date -d @1700000000
来源：http://hz.52xcode.cn/gtqxeohfov.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtmpxpnhse.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yonumen.top/gttinvxiin.html

[R72] 等待端口就绪
来源：http://hz.birdmap.top/gtzkpepler.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gzhubu.top/gtvyvegcza.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtmfruxbvb.html

split -l 1000 big.log part_
来源：http://hz.jyoumei.cn/gtoxwwyekd.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gttzjxwalq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gtbnhcwxse.html

[R75] 导出环境变量
来源：http://hz.pengpengdd.cyou/gtnvmfhxbw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.iojbl.cn/gtzbmzsnzf.html

[R76] 使用临时文件
来源：http://hz.aibaodan.cn/gtjoqfuqfo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtvrlvggff.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtjvjkfwyc.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gtdtkdbphq.html

[R78] 交互式菜单
来源：http://hz.jiagoushi.top/gtyeyizodd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gtckdslthl.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtdbtzpqxc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtkkjcyszz.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtjizatqtl.html

time ./run.sh
来源：http://hz.daxiang520.top/gthpdpbmqa.html

================================================================================
来源：http://hz.jqgfzy.top/gtjljgtipy.html

S. C / C++ 专题
来源：http://hz.gaohongyu789.top/gtfqwdmzri.html

================================================================================
来源：http://hz.jianghu66.top/gtrvmgrdwz.html

[S01] C：Hello World
来源：http://hz.xziqi.cn/gtdtbswgti.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtdimbiole.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtenxbudyv.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gtbosnmrlc.html

int a = 10; printf("%d\n", a);
来源：http://hz.quarkkingdee.top/gtafasrqaq.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gtdepbiedz.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtgsuneqww.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtzvslohmr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gzhubu.top/gthfvbzhek.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtnknzdwuz.html

strlen(s)
来源：http://hz.ydjk.org.cn/gtcvyntzmp.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gtbgflfmre.html

strcmp(a, b) == 0
来源：http://hz.hnqzz.top/gtjivinwte.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gttchahzzp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.svipenyu.cn/gtccjfnrkj.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258.top/gtpsrkheyd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenzaomai.com/gtiourebwz.html

[S09] C：结构体定义与初始化
来源：http://hz.vqdsnc.cn/gtjwqqqxal.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.iojbl.cn/gtnoujimsi.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtouwklyyb.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtmhjqrfzh.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gteatsvoim.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dashuyun.cn/gtizrljzof.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.quarkkingdee.top/gtljgzvczp.html

fclose(f);
来源：http://hz.redwolf501.top/gtckgekqfx.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtfyumsckk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cdnleiting.top/gtsegrqklf.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gtyrodohha.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ivvv.top/gtrggqcnjz.html

[S14] C：枚举
来源：http://hz.nwbrower.top/gtgpkaedps.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.svipenyu.cn/gtzpltjphe.html

[S15] C：类型转换
来源：http://hz.yanxiufei.cn/gtvfbjwffo.html

(double) a / b
来源：http://hz.yangfankeji.com/gtyxvzryhf.html

[S16] C：位操作置位
来源：http://hz.zhengqikj.top/gtvqlgcrpo.html

x |= (1 << 3);
来源：http://hz.mhx1999.top/gtctlxbgxh.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258.top/gthdnbneqj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhengqikj.top/gtxdumolsj.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtqduaekcx.html

int main(int argc, char **argv)
来源：http://hz.bjfxy.top/gtovzuqwzm.html

[S19] C：快速排序
来源：http://hz.gotoacloud.top/gtszsbcuuy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gthsppyojf.html

[S20] C：二分查找
来源：http://hz.jlsjyb.cn/gtpmanjgwo.html


<!-- 参考信息 -->