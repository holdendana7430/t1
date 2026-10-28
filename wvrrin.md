代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtwuvynbmk.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtrrkdjren.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gteelvefmc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cucudq.cn/gtmjxtocaq.html

[Q61] 移动平均
来源：http://hz.redwolf501.top/gtnlwgapnm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtohyuyjdf.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gttbcvgwkf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtfeucpnll.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtwxxxjysp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangkeji.top/gtamfkaaqt.html

[Q64] 提交事务
来源：http://hz.hongshengwenyu.top/gtjqixnvgz.html

COMMIT;
来源：http://hz.jlsjyb.cn/gttthtiavc.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gtzusjsuxf.html

ROLLBACK;
来源：http://hz.yanxiufei.cn/gthqjsivry.html

[Q66] 行锁查询
来源：http://hz.haohaochexian.top/gtmxlvxucr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gtewverlln.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtopfbyxoz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gtbxqxstno.html

[Q68] 保存点
来源：http://hz.yj202588.top/gtrguuqwhz.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtprpxlwbh.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtsmyuhgcb.html

[Q69] 查看执行计划
来源：http://hz.xingfuxueyuan.xyz/gtwuzevwte.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtgejfmvvb.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtkgyspply.html

ANALYZE TABLE users;
来源：http://hz.gogol.net.cn/gtqqotncdo.html

[Q71] 查看建表语句
来源：http://hz.hnqzz.top/gtxrqusdzs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yangfankeji.com/gtxpokehtv.html

[Q72] 查看索引
来源：http://hz.ydzc1.top/gtfvgwynlq.html

SHOW INDEX FROM users;
来源：http://hz.guowangkeji.top/gtzebsqhzs.html

[Q73] 查看表状态
来源：http://hz.haohaochexian.top/gtanchcfiw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.9152youxi.cn/gtwcfawcgr.html

[Q74] 强制使用索引
来源：http://hz.jlsjyb.cn/gtczzymbkn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxuanxn.top/gtlxzrdtjm.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gtutahydin.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xziqi.cn/gthuxnptee.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtrdtpesio.html

[Q76] 按天统计
来源：http://hz.yongpay.top/gtzvybmysl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtfokzqhdm.html

[Q77] 时间加减
来源：http://hz.ivvv.top/gttfwnvvfr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtobqrwgqu.html

[Q78] 当前时间
来源：http://hz.ywan-chungtsiang.top/gtixfcenpm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xinyue.icu/gtdgiamxtq.html

[Q79] 字符串拼接
来源：http://hz.ppjwa.cn/gtgxgirxyn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtqdbisixc.html

[Q80] 字符串截取
来源：http://hz.wangdashe.top/gtlceosrut.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtnnnnusmq.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtxzbteqzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258.top/gtgujxzokp.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gtmodwruft.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuanzx.com/gtmplibcca.html

[Q83] 大小写转换
来源：http://hz.c1oappe.top/gtmmjboxvz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhengqikj.top/gtapccllvl.html

[Q84] 去除首尾空格
来源：http://hz.zhongyouzk.top/gtvrufrmlg.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtjceajyeq.html

[Q85] 数值取整
来源：http://hz.bjfxy.top/gtvdvjrjsx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtoljinjjq.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gtvxeqwesq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xinyue.icu/gtnucjejwl.html

[Q87] JSON 字段做条件
来源：http://hz.jianghu66.top/gtvqvdhpbo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.quarkkingdee.top/gtcuahszxc.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtoxwjwtvs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yangfankeji.com/gtcuglvpgr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtqoxbreoo.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtgcomimwb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtywatjzye.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtjbntzdzz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cucudq.cn/gtgiqxmpaw.html

================================================================================
来源：http://hz.tanke756.top/gtymegtrmh.html

R. Bash 专题
来源：http://hz.nanxinkj.top/gtdbthvjus.html

================================================================================
来源：http://hz.bjfxy.top/gtekqptjhd.html

[R01] shebang 与严格模式
来源：http://hz.9152youxi.cn/gtrpqsvuqz.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtaljxmzcl.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtwmtzeows.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gthjlnomyf.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtyzsmgmbs.html

[R03] 只读变量
来源：http://hz.aibaodan.cn/gtljthymjw.html

readonly PI=3.14
来源：http://hz.hfpthk.cn/gtejmpvmhr.html

[R04] 位置参数
来源：http://hz.vqdsnc.cn/gtrpiwdabr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ppjwa.cn/gtkvjulqwx.html

[R05] 参数默认值
来源：http://hz.tian-w.cn/gtamvhleed.html

name="${1:-default}"
来源：http://hz.shzxlz.cn/gtbepqxfcn.html

[R06] 判断命令是否存在
来源：http://hz.c1oappe.top/gtrlhfadyh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.c1oappe.top/gtnffkbwgs.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtbrwykhfj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtgkfsxbja.html

[R08] 数值比较
来源：http://hz.gotoacloud.top/gtzbvefbyb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenjidiqi.icu/gtrlkapqtr.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gttwfpdlkt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gttocxquov.html

[R10] 正则匹配
来源：http://hz.ppjwa.cn/gtsohkvnbj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ivvv.top/gtehxffjwt.html

[R11] case 多分支
来源：http://hz.hysaishi.cn/gtxzqcdwid.html

case "$1" in
来源：http://hz.haohaochexian.top/gtffybgqrr.html

start) echo "启动" ;;
来源：http://hz.0kj1m.cn/gtbgykpojb.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gteztfexzz.html

*)     echo "未知命令" ;;
来源：http://hz.pycfn.com/gtrwmsioes.html

esac
来源：http://hz.ydjk.org.cn/gtermfvsgi.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtkmmtkijq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtqcicwuuc.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtaayafdum.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fzhhl.top/gteainpfof.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtgrtmrkyy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtvzpjghwc.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gthlbpkkkq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.mhx1999.top/gtpruybfdl.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gthwwrnahu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gtmictgait.html

[R17] 数组定义与取值
来源：http://hz.zdqjudy.top/gthbkptykt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.birdmap.top/gtzdyseivu.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gtcxcsayjx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtuberubmn.html

[R19] 数组长度
来源：http://hz.ehwqpu.com/gtpciuvqcj.html

echo "${#arr[@]}"
来源：http://hz.zhijiandao.cn/gtrzidweby.html

[R20] 关联数组（字典）
来源：http://hz.feifeiyinyue.top/gtkiqlwzqr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtveuyeffz.html

[R21] 字符串长度
来源：http://hz.yvedp.cn/gthekvaevp.html

echo "${#s}"
来源：http://hz.wangdashe.top/gtjdgfsces.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gtanyptznp.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtxzuipkpn.html

[R23] 字符串替换
来源：http://hz.jlsjyb.cn/gtkworufbn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigufen.top/gtbefazaub.html

[R24] 大小写转换
来源：http://hz.svipenyu.cn/gtonppdzhm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yonumen.top/gtonbdvxhy.html

[R25] 去后缀 / 去前缀
来源：http://hz.nwbrower.top/gtccpffsqb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.andypj.xyz/gttcdjipbx.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtcycrsvna.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gtxcnggvqb.html

[R27] 算术展开
来源：http://hz.fzhhl.top/gttkulyfot.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtpfskqaev.html

[R28] 浮点运算
来源：http://hz.9152youxi.cn/gtkefelpwj.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtecbgycpy.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gthtfjhtng.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yangfankeji.com/gtvlpdtach.html

[R30] 函数返回状态码
来源：http://hz.kuanghao11.cn/gthgjqpeom.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tianlin.xyz/gtahjorksk.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtwbucxcny.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtcodloarc.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtbuiehabv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.0kj1m.cn/gtqzeeyvtt.html

[R33] 捕获错误并提示行号
来源：http://hz.guowangkeji.top/gtwtlnskho.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuetiantiany.cn/gtcopjmoew.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtoqwsjzut.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtlgsjegxv.html

[R35] 后台执行并等待
来源：http://hz.yj20258.top/gtfixlxmvg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cashguo.top/gtjxraxxrs.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtuuzpuzxr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guowangkeji.top/gtwdoivpwm.html

[R37] 把输出赋给变量
来源：http://hz.shangyingyoupin.top/gtoiaqlbqu.html

files=$(ls -1)
来源：http://hz.feifeiyinyue.top/gtfnryxkhg.html

[R38] 管道串联
来源：http://hz.svipenyu.cn/gtqnsuhalw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yangfankeji.com/gtqgobnovl.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258.top/gtpvttdhkp.html

cmd > out.log 2>&1
来源：http://hz.daria6918.cn/gtwodnewat.html

[R40] 追加写日志
来源：http://hz.kuanghao11.cn/gtqcruwpaf.html

echo "log" >> out.log
来源：http://hz.9152youxi.cn/gtpmijfusp.html

[R41] 丢弃输出
来源：http://hz.yvedp.cn/gtivvbrgvw.html

cmd >/dev/null 2>&1
来源：http://hz.yuanzhike.top/gtjobmuhlw.html

[R42] 输入重定向
来源：http://hz.nanxinkj.top/gtfzywuipg.html

wc -l < a.txt
来源：http://hz.shanyushiyangtech.top/gtvwaiaccl.html

[R43] 按名字查找文件
来源：http://hz.yanxiufei.cn/gtwwuudlik.html

find . -name "*.log" -type f
来源：http://hz.sweek.top/gtxucdxtps.html

[R44] 按修改时间查找
来源：http://hz.hongshengwenyu.top/gtqibegsga.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtjwshcfak.html

[R45] 批量删除
来源：http://hz.hfpthk.cn/gtmyuykhwl.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtcotnhgzb.html

[R46] 递归替换文件内容
来源：http://hz.ppjwa.cn/gtwxcdbipw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zycfv.cn/gtbldpmabd.html

[R47] sed 单行替换
来源：http://hz.gogol.net.cn/gtoaexbpro.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtubxvyzcn.html

[R48] awk 取指定列
来源：http://hz.iojbl.cn/gtypsirgwl.html

awk '{print $1, $3}' a.txt
来源：http://hz.andypj.xyz/gtvhxjnmrx.html

[R49] awk 带条件
来源：http://hz.jqgfzy.top/gthtqkmsgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tianlin.xyz/gtxsszvaha.html

[R50] awk 求和
来源：http://hz.sweek.top/gttektjpta.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtwylxndsk.html

[R51] 排序去重取前几
来源：http://hz.ywan-chungtsiang.top/gtdawdexbk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yvedp.cn/gtfiomskib.html

[R52] 统计行数
来源：http://hz.guowangkeji.top/gtfjbdhfwg.html

wc -l a.txt
来源：http://hz.ywan-chungtsiang.top/gtbdodxuwo.html

[R53] 查看文件头与实时尾
来源：http://hz.andypj.xyz/gtjzzamrqc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhongyouzk.top/gtkwtcbabe.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtjyfsdojr.html

diff a.txt b.txt
来源：http://hz.nanxinkj.top/gtyflptose.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtlnxtzrnu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtbwspiynw.html

[R56] 远程拷贝
来源：http://hz.jinqigfzy.top/gtwdehnzgq.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtdkepbzmf.html

[R57] 远程执行命令
来源：http://hz.chenzaomai.com/gtqaeaadon.html

ssh user@host 'uptime'
来源：http://hz.zhijiandao.cn/gtcedczzmo.html

[R58] 下载文件
来源：http://hz.yanxiufei.cn/gteovpymtq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtmpwpvqxj.html

[R59] 发 POST JSON
来源：http://hz.zhijiandao.cn/gttyhvxhei.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtbywlsmzc.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtbzmxkzpk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yanxiufei.cn/gtabogquhq.html

[R61] 磁盘占用
来源：http://hz.jqgfzy.top/gtouxefvkm.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtzprzblvw.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangkeji.top/gtaqpfnbes.html

du -ah . | sort -rh | head -10
来源：http://hz.c1oappe.top/gtpuvzovxr.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtpnxlcjpb.html

free -h;  ps aux | grep nginx
来源：http://hz.tian-w.cn/gtaktlsxlc.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtwsokkcfh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tanke756.top/gtqtobwrcg.html

[R65] 查看端口占用
来源：http://hz.yj20258.top/gtgqvsmnqq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtkszfjdry.html

[R66] 定时任务
来源：http://hz.yanxiufei.cn/gtphupqrcu.html

crontab -e;  crontab -l
来源：http://hz.sufxvd.cn/gtgarvceaf.html

[R67] 生成随机十六进制串
来源：http://hz.dianchejie.cn/gtflbjtlgu.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gtownxgtdc.html

[R68] 计算文件校验值
来源：http://hz.redwolf501.top/gtnlmqjbgw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtjuzmrdqm.html

[R69] 生成随机密码
来源：http://hz.yangfankeji.com/gtqlquqweo.html

head -c 16 /dev/urandom | base64
来源：http://hz.andypj.xyz/gtjsdokguy.html

[R70] 时间戳与互转
来源：http://hz.yj20258.top/gtwntxwzjj.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gtwdbdkjpm.html

[R71] 日期格式化
来源：http://hz.andypj.xyz/gtqsnprdvm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenjidiqi.icu/gtbrmrylhp.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtjjqupxbi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenzaomai.com/gtxpxurfkl.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtehnqnexn.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtzxozfisu.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtjtzbprkr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtvscistzl.html

[R75] 导出环境变量
来源：http://hz.yueranfly.top/gtwcakfuff.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangkeji.top/gtlekeaaav.html

[R76] 使用临时文件
来源：http://hz.yuxming.cn/gttzoewauh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gtssnmzjeu.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtlsjldguw.html

read -rp "请输入: " ans
来源：http://hz.gaohongyu789.top/gtohgyjzwn.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtteuznbdq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gtaggsnfzs.html

[R79] 解析命令行选项
来源：http://hz.zycfv.cn/gtukkbactd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtxemngydu.html

[R80] 查看脚本执行耗时
来源：http://hz.hysaishi.cn/gtglacniaj.html

time ./run.sh
来源：http://hz.sweek.top/gtwuledtny.html

================================================================================
来源：http://hz.daxiang520.top/gtvvoogyos.html

S. C / C++ 专题
来源：http://hz.cucudq.cn/gtiqmzvmqk.html

================================================================================
来源：http://hz.cdnleiting.top/gtkbteqeil.html

[S01] C：Hello World
来源：http://hz.shangyingyoupin.top/gtadxucsvc.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtdbjqsrox.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtoresxxgo.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gthvshearo.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtznrolkec.html

[S03] C：读入整数
来源：http://hz.fzhhl.top/gtuvdyvthd.html

int x; scanf("%d", &x);
来源：http://hz.cheryme.top/gtweiwbjra.html

[S04] C：字符串复制
来源：http://hz.jiagoushi.top/gtbtdpglny.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtfjeeclsl.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtsxxnoxma.html

strlen(s)
来源：http://hz.xuanzx.com/gttqnhavdd.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtreuclmnf.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtbiuhglyl.html

[S07] C：数组遍历求和
来源：http://hz.mhx1999.top/gtjtlckeqf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtlxdfksmo.html

[S08] C：动态内存分配与释放
来源：http://hz.hammf.cn/gtubqrquae.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtyfovptxx.html

[S09] C：结构体定义与初始化
来源：http://hz.yangfankeji.com/gtcpxxucas.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gtwpekxvax.html

[S10] C：指针与解引用
来源：http://hz.xuanzx.com/gtnackotva.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtrauvjraz.html

[S11] C：逐行读文件
来源：http://hz.cashguo.top/gtfwkaxlix.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinghuilouyu.cn/gtmgviahjp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtpekqsfll.html

fclose(f);
来源：http://hz.aibaodan.cn/gtuahpxryx.html

[S12] C：写文件
来源：http://hz.quarkkingdee.top/gtnkeojvuk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gtgmeqyyoh.html

[S13] C：宏定义
来源：http://hz.yj202588.top/gtmldgcsqh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gtnmgnimxe.html

[S14] C：枚举
来源：http://hz.cqqwz.cn/gtlxgwwzsk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gtduszmexf.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtjfosqzsp.html

(double) a / b
来源：http://hz.cheryme.top/gtkbppocll.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtfhqqrjbx.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtqbkysnjj.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gttbnlbmjt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtqhwcbovt.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtrflvvkrh.html

int main(int argc, char **argv)
来源：http://hz.tanke756.top/gtaautksfl.html

[S19] C：快速排序
来源：http://hz.316326.xyz/gtfsoladcb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtovohkrgk.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtonwmhpgb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtaidohprk.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtrcacjygu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gthvwzzudb.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtrsajuygm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gtidhxmjxb.html

[S23] C：随机数
来源：http://hz.hammf.cn/gtkurlxgzu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pycfn.com/gtdchumjtv.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtbpbbxmwe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtqvlyoklp.html

[S25] C：内存拷贝
来源：http://hz.hywenlv.cn/gtcqtulwiq.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtwrjsptaq.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtgqgiwetq.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gthlglcuxy.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtaaobaxao.html

const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtticrkqjj.html

[S28] C：静态变量
来源：http://hz.daria6918.cn/gtoqokwwwq.html

static int counter = 0;
来源：http://hz.nanxuanxn.top/gthbhnagva.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtndepjqan.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ybcxt.top/gtpsxvlvrr.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gtdxlwywxv.html


<!-- 参考信息 -->