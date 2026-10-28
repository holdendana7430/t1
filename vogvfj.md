代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtthfpcvyx.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtqzraoxfy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gtdafjskbg.html

[Q53] 按条件删除
来源：http://hz.sweek.top/gtjqdzqrev.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gtasdatgwb.html

[Q54] 清空表
来源：http://hz.aibaodan.cn/gtnvmpwrgj.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtncsfctdv.html

[Q55] 排名（并列占位）
来源：http://hz.wangshuangyany.cn/gtzvluounu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtpuxagcye.html

[Q56] 密集排名（并列不占位）
来源：http://hz.iojbl.cn/gtxiywosql.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtwempbkwk.html

[Q57] 行号
来源：http://hz.xingfuxueyuan.xyz/gtnujfnrst.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxuanxn.top/gtqrdypsnu.html

[Q58] 累计求和
来源：http://hz.zhixingplan.top/gtiumdbagm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yangfankeji.com/gtdnvvcvuo.html

[Q59] 分组内累计
来源：http://hz.dianchejie.cn/gtijtairqv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gtfsatepqb.html

[Q60] 取上一行 / 下一行
来源：http://hz.shangyingyoupin.top/gtaesyqvin.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuetiantiany.cn/gtwwqyxiyp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gtsgblhxmz.html

[Q61] 移动平均
来源：http://hz.zdqjudy.top/gtkmiheliu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtkbfzopbo.html

[Q62] 分组占比
来源：http://hz.tian-w.cn/gtiqiyqfwg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gthtgsggrl.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gtixstfwvx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.pycfn.com/gtjsmxhtwr.html

[Q64] 提交事务
来源：http://hz.ywan-chungtsiang.top/gtvitthcwx.html

COMMIT;
来源：http://hz.gzhubu.top/gtmitrgiqd.html

[Q65] 回滚事务
来源：http://hz.jqgufenzy.top/gtslngyiit.html

ROLLBACK;
来源：http://hz.hammf.cn/gtqcxgfxiz.html

[Q66] 行锁查询
来源：http://hz.zhiwuduotai.top/gtzxkxooed.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.316326.xyz/gtuhsnznwe.html

[Q67] 设置隔离级别
来源：http://hz.ydjk.org.cn/gtmgibblwc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.9152youxi.cn/gtklvpkdhw.html

[Q68] 保存点
来源：http://hz.hnqzz.top/gtkgnhqmks.html

SAVEPOINT sp1;
来源：http://hz.pycfn.com/gtsryaizrw.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtyqlenqdp.html

[Q69] 查看执行计划
来源：http://hz.yonumen.top/gtfktlktxx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gtkfucupnb.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gtqdcskpmd.html

ANALYZE TABLE users;
来源：http://hz.ehwqpu.com/gtyclzfsli.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtwkddbhoj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aizwys.cn/gtgwmcumiu.html

[Q72] 查看索引
来源：http://hz.zhiwuduotai.top/gtmdxombwn.html

SHOW INDEX FROM users;
来源：http://hz.0kj1m.cn/gtdgcarqmk.html

[Q73] 查看表状态
来源：http://hz.guannengcc.top/gtqnjobtph.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtvpsvgpud.html

[Q74] 强制使用索引
来源：http://hz.mhx1999.top/gtowdjsbjo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenzaomai.com/gtlzgbnfvg.html

[Q75] 日期格式化
来源：http://hz.fzhhl.top/gthxgapyor.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.316326.xyz/gtmbuaheaa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.52xcode.cn/gtboeeoiel.html

[Q76] 按天统计
来源：http://hz.jqgfzy.top/gtqzejnlyf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtsqilfckx.html

[Q77] 时间加减
来源：http://hz.chenlongwang.top/gtqihtzeee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ybcxt.top/gtqnijbawb.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtpwqfiqsz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gtvazqbmfm.html

[Q79] 字符串拼接
来源：http://hz.zhoulong.xyz/gtjjlumejl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtwlepwcme.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtrhkrcxmg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fzhhl.top/gtdcpcqjyd.html

[Q81] 字符串替换
来源：http://hz.wangdashe.top/gtfsmzuksd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtflxmwtjh.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtaswzeljv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pycfn.com/gtgixtbxli.html

[Q83] 大小写转换
来源：http://hz.dianchejie.cn/gtmnzhppls.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtrnyssvua.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtwxctnbur.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtlykytyim.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gtylpqsrhl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gtglxicuej.html

[Q86] 读取 JSON 字段
来源：http://hz.c1oappe.top/gtgmycoaze.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtvjzpyagk.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gtlqcixvfj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtpgsjhfgt.html

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gtpobrsmza.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gthuqekruk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jyoumei.cn/gtgujrktgl.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtsaqbwopa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtqjaojbmd.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtuhlebkub.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.haohaochexian.top/gtpygtqcvj.html

================================================================================
来源：http://hz.cashguo.top/gtknbnesur.html

R. Bash 专题
来源：http://hz.yvedp.cn/gtzuweuure.html

================================================================================
来源：http://hz.tian-w.cn/gtiavhmtci.html

[R01] shebang 与严格模式
来源：http://hz.pengpengdd.cyou/gtnwpfsiwa.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtfznbqdtt.html

set -euo pipefail
来源：http://hz.zycfv.cn/gthcvdredz.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtbhokohwx.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gttikcrqae.html

[R03] 只读变量
来源：http://hz.yueranfly.top/gtezbloxev.html

readonly PI=3.14
来源：http://hz.jyoumei.cn/gtqwmtetfd.html

[R04] 位置参数
来源：http://hz.xylfe.cn/gtwshmscna.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigufen.top/gtlwxcmqjv.html

[R05] 参数默认值
来源：http://hz.yueranfly.top/gtbvcvrboz.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtetofksla.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtxnjtfzch.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.0kj1m.cn/gtenmaoroj.html

[R07] if 判断文件
来源：http://hz.snrcjt.cn/gtcdzrzftl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gteotlabge.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtqnyzvfpo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtbqkkhywd.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtdjmbpwoi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gttqoomikg.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtjospgrpj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gtiubhukhz.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gtolspbfft.html

case "$1" in
来源：http://hz.shangyingyoupin.top/gtkeugxycd.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtuvpulcsu.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtemjuycjm.html

*)     echo "未知命令" ;;
来源：http://hz.zhixingplan.top/gtsyjfntiv.html

esac
来源：http://hz.tianlin.xyz/gtbiieoweb.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gtglgagwdh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangkeji.top/gtdulxombh.html

[R13] for 计数循环
来源：http://hz.gogol.net.cn/gtdpewrcea.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gttyxumusm.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtlmbhkfjz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guannengcc.top/gttzgrgcfv.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtsiijrkhs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hysaishi.cn/gtpvelzpnk.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtadyxakjn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtyoqhythd.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtyasexyof.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gttdwhbihq.html

[R18] 遍历数组
来源：http://hz.zycfv.cn/gtqkdoeykm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtzvsyynty.html

[R19] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtzqvmbdpn.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtyecfnqgd.html

[R20] 关联数组（字典）
来源：http://hz.dashuyun.cn/gtllmjzuem.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ybcxt.top/gtufohbmae.html

[R21] 字符串长度
来源：http://hz.bjfxy.top/gtuitinldb.html

echo "${#s}"
来源：http://hz.yvedp.cn/gteogzmmpi.html

[R22] 截取子串
来源：http://hz.chenzaomai.com/gticschmnu.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtnfwjimyd.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtedqhtxmf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gogol.net.cn/gtfluxtude.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtslptdejb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gttjcgbpxn.html

[R25] 去后缀 / 去前缀
来源：http://hz.pycfn.com/gtktfrtnmh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gtzqmataav.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtzuswijpr.html

now=$(date +%F); echo "$now"
来源：http://hz.iojbl.cn/gtuajtcvds.html

[R27] 算术展开
来源：http://hz.zhaomingkeji.xyz/gtmgilvjoz.html

echo $((1 + 2 * 3))
来源：http://hz.hongshengwenyu.top/gtjoklghwf.html

[R28] 浮点运算
来源：http://hz.yangfankeji.com/gtvqpobvad.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gtqkzvasbo.html

[R29] 定义函数
来源：http://hz.jianghu66.top/gtovcfupdp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydjk.org.cn/gtujsiwhjm.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtostgpfpi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtijferpae.html

[R31] 局部变量
来源：http://hz.birdmap.top/gtddidhnch.html

f() { local x=1; echo "$x"; }
来源：http://hz.gaohongyu789.top/gtyepnwwso.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gtaqzwiiws.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cdnleiting.top/gthkbfkgwu.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gtsanfwpan.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydzc1.top/gtosdomtad.html

[R34] 退出时清理
来源：http://hz.smart0.xyz/gtxkvzwnfr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gthyzxjkds.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtelvirbpr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydjk.org.cn/gtjrzlwwpd.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtxqfhsexs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dianchejie.cn/gtkeyidcac.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gttkehpiuz.html

files=$(ls -1)
来源：http://hz.nanxinkj.top/gtdddvktwf.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtjfzeczbz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gogol.net.cn/gtpzrhkmdv.html

[R39] 重定向标准输出与错误
来源：http://hz.xuetiantiany.cn/gtmshdipzb.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtktkkyeid.html

[R40] 追加写日志
来源：http://hz.wangshuangyany.cn/gtcqoxyvst.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtbdovrrvj.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gtujnfoqgw.html

cmd >/dev/null 2>&1
来源：http://hz.jlsjyb.cn/gtzlppthgc.html

[R42] 输入重定向
来源：http://hz.xuanzx.com/gtraqgwmre.html

wc -l < a.txt
来源：http://hz.hysaishi.cn/gtldrfnqyq.html

[R43] 按名字查找文件
来源：http://hz.sufxvd.cn/gtdlrzmwey.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtxuuylrqf.html

[R44] 按修改时间查找
来源：http://hz.pengpengdd.cyou/gtefjqfzbi.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtnmlnbrqh.html

[R45] 批量删除
来源：http://hz.chenlongwang.top/gtnrbbonze.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gtkxumlgfe.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtokcyhfuk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtrrqfjcxi.html

[R47] sed 单行替换
来源：http://hz.jqgufenzy.top/gtvoovrses.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhongyouzk.top/gtcxweapeo.html

[R48] awk 取指定列
来源：http://hz.daxiang520.top/gtpieinuwi.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtvopvxfbj.html

[R49] awk 带条件
来源：http://hz.52xcode.cn/gtmlarlyay.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fengsongda.top/gtkksmwqde.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtdmtykjjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nanxuanxn.top/gtwbpeqqhj.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtqqtytinz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gtdacjygtz.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gtbotjmsmm.html

wc -l a.txt
来源：http://hz.shuidangran.top/gtwjrbzsme.html

[R53] 查看文件头与实时尾
来源：http://hz.cqqwz.cn/gtnoiwzdva.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtjpnmfeni.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtugzffbss.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gttsbtofdt.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtnekrkulr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtjhwtpbrg.html

[R56] 远程拷贝
来源：http://hz.nanxuanxn.top/gtwlxnuacr.html

scp file user@host:/path/
来源：http://hz.yuxming.cn/gtgqlndhfp.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtpmptcsca.html

ssh user@host 'uptime'
来源：http://hz.tianlin.xyz/gtobfhruxe.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtwgoionfm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtkeojoham.html

[R59] 发 POST JSON
来源：http://hz.xylfe.cn/gtjdtumcrb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.svipenyu.cn/gtishgrqai.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtgsqyvkwl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtgeltshbw.html

[R61] 磁盘占用
来源：http://hz.ppjwa.cn/gtpfvkcjyo.html

df -h;  du -sh *
来源：http://hz.cdnleiting.top/gtqddfgouo.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gtemzkarqf.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgufenzy.top/gtzrfwtnmx.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gtffsultcf.html

free -h;  ps aux | grep nginx
来源：http://hz.bjfxy.top/gtshdofxzu.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtdeenvgsg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yanxiufei.cn/gtmxqfblui.html

[R65] 查看端口占用
来源：http://hz.andypj.xyz/gtorlxpqdc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nanxinkj.top/gtcdopzahq.html

[R66] 定时任务
来源：http://hz.yuanzhike.top/gtdnsyvpkv.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtecbefrfw.html

[R67] 生成随机十六进制串
来源：http://hz.meibo888.top/gtoqtmthju.html

openssl rand -hex 16
来源：http://hz.hammf.cn/gtckmtccqk.html

[R68] 计算文件校验值
来源：http://hz.cheryme.top/gtphytzcij.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.meibo888.top/gtvytzkwey.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtzpsmrsng.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gtftrtfvlw.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtenerttdt.html

date +%s;  date -d @1700000000
来源：http://hz.zhaomingkeji.xyz/gtfqmfpgup.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtpwpqsmbg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtgvkqewji.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtfhlmdwyv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtveukjxzp.html

[R73] 分割大日志
来源：http://hz.yuanzhike.top/gtpmaqzdsv.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtpzrpdtgr.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtilejflhn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtqcohxscy.html

[R75] 导出环境变量
来源：http://hz.shzxlz.cn/gtleijrvcl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtftgtrfbo.html

[R76] 使用临时文件
来源：http://hz.hywenlv.cn/gthlrolaum.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gttnpphdjt.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtfzbiemwy.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtuldixvkx.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangkeji.top/gtjmfebldi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtiffnkwoj.html

[R79] 解析命令行选项
来源：http://hz.ydjk.org.cn/gtvyzrykyw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pycfn.com/gtfndoanqy.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gtjiaawvsq.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtpixgjskd.html

================================================================================
来源：http://hz.sysykeji.top/gtamylzciv.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtcwdensgq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtpxcflmoy.html

[S01] C：Hello World
来源：http://hz.zhijiandao.cn/gtliknqvao.html

#include <stdio.h>
来源：http://hz.quarkkingdee.top/gtscxntacp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtrhzeivms.html

[S02] C：变量与格式化输出
来源：http://hz.jinyuanbaomall.cn/gtngeijznw.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtomxwrwuf.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtrabdoxjy.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtpgcmeugm.html

[S04] C：字符串复制
来源：http://hz.xuetiantiany.cn/gtmucrggqz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangtech.top/gtaocsoodl.html

[S05] C：字符串长度
来源：http://hz.feifeiyinyue.top/gtbckrbicj.html

strlen(s)
来源：http://hz.ydjk.org.cn/gthkyjcjpu.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtxtjnsqyo.html

strcmp(a, b) == 0
来源：http://hz.havefunace.top/gtyfkrhbdv.html

[S07] C：数组遍历求和
来源：http://hz.hfpthk.cn/gttspzjiop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigufen.top/gtgiufgixm.html

[S08] C：动态内存分配与释放
来源：http://hz.yangfankeji.com/gtisasfeyc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gtpytzmkha.html

[S09] C：结构体定义与初始化
来源：http://hz.tianlin.xyz/gtowacsexy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hfpthk.cn/gtlxpzivdw.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtvwcdynir.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtgztxknrj.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtqvpijulu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xylfe.cn/gtnidfqaea.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cashguo.top/gtpopwfpso.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtihjildgr.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtdoyuwfsb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gtdklkuxpy.html

[S13] C：宏定义
来源：http://hz.birdmap.top/gtnpbocdvl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xziqi.cn/gtswrhnmny.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtsglcjiaq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtzhsfnnqt.html

[S15] C：类型转换
来源：http://hz.cucudq.cn/gtqppiitiv.html

(double) a / b
来源：http://hz.meibo888.top/gtrfbpayig.html

[S16] C：位操作置位
来源：http://hz.cucudq.cn/gtxslkajwm.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtwnbyxaca.html

[S17] C：安全拼接字符串
来源：http://hz.shuidangran.top/gtptwmpedj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.havefunace.top/gtlfuubbws.html

[S18] C：命令行参数
来源：http://hz.yuanzhike.top/gtmmxlmmdx.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtojupmqxx.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtejqepoja.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtvonqvenw.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gtrryclewk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtqatjauko.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtflsnjonz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtrflypkbi.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtgcwnhffu.html


<!-- 参考信息 -->