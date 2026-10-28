代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtzwyayaxi.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtenijazbn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gttdjqdpsn.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtwbdavapv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cheryme.top/gtzhhdbbjn.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuanzx.com/gtrmadhfoc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jianghu66.top/gtwrhrfqfc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.snrcjt.cn/gthbhciyzk.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtcjiximsf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtmpcwtmxw.html

[Q62] 分组占比
来源：http://hz.kuanghao11.cn/gthbzyurli.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtsniovojh.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtwhwlqrym.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gtxpmhamef.html

[Q64] 提交事务
来源：http://hz.vqdsnc.cn/gtpmuqlpro.html

COMMIT;
来源：http://hz.daria6918.cn/gtesywqnvr.html

[Q65] 回滚事务
来源：http://hz.yj20258.top/gtsoewktpc.html

ROLLBACK;
来源：http://hz.cashguo.top/gtdteprmpc.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtbsryxwzu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtocxyvaqi.html

[Q67] 设置隔离级别
来源：http://hz.nanxuanxn.top/gtzprjolfy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gtwrsanuzz.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtpbosbwcf.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtldamdbvd.html

ROLLBACK TO sp1;
来源：http://hz.cdnleiting.top/gteibczvyr.html

[Q69] 查看执行计划
来源：http://hz.haohaochexian.top/gthnivxrly.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangshuangyany.cn/gtuufilnus.html

[Q70] 更新统计信息
来源：http://hz.zhengqikj.top/gtbtdmsqqx.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gturowylcw.html

[Q71] 查看建表语句
来源：http://hz.yj20258.top/gtahqludaj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtogryancu.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtflifexdj.html

SHOW INDEX FROM users;
来源：http://hz.guowangkeji.top/gtikcoqdme.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtckhkucat.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtqkvftfce.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtttwtruaq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenzaomai.com/gtyifekcrv.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtuovbvzns.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtklsdmryw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinghuilouyu.cn/gtoagzwxbu.html

[Q76] 按天统计
来源：http://hz.hfpthk.cn/gtqxzknepl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gthycpqkvx.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtkgmximtt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhijiandao.cn/gtylkzufdz.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtnizytnhq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtyqmbwkjl.html

[Q79] 字符串拼接
来源：http://hz.wangshuangyany.cn/gtxjitvkoh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cqqwz.cn/gtukcqevur.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtotsnqtla.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daria6918.cn/gtjtylccoo.html

[Q81] 字符串替换
来源：http://hz.jiagoushi.top/gtbbzggzvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangshuangyany.cn/gtiwyybbkt.html

[Q82] 字符长度与字节长度
来源：http://hz.aizwys.cn/gthtupfuit.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258888.top/gtrtpnvleu.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gtpykxfego.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.andypj.xyz/gtmumsexxr.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtasxunjip.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtxkmfvmwh.html

[Q85] 数值取整
来源：http://hz.mhx1999.top/gtgdrjfzdv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghu66.top/gtslmsfvlg.html

[Q86] 读取 JSON 字段
来源：http://hz.vqdsnc.cn/gtxpgshwyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.smart0.xyz/gtpwlqmvtl.html

[Q87] JSON 字段做条件
来源：http://hz.andypj.xyz/gtwxckpfob.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gotoacloud.top/gtzybaflka.html

[Q88] 行转列（条件聚合）
来源：http://hz.guowangkeji.top/gtllgfublk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yonumen.top/gtwdwqodtk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxinkj.top/gtvkbkgxfl.html

[Q89] 判断表是否存在
来源：http://hz.xylfe.cn/gtojsrwkno.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.meibo888.top/gtrznkhfhx.html

[Q90] 生成序号列
来源：http://hz.wangdashe.top/gtvwdswxjg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.andypj.xyz/gtivdmcbfx.html

================================================================================
来源：http://hz.yonumen.top/gtehjvxoju.html

R. Bash 专题
来源：http://hz.hnxiangtu.top/gttliwirem.html

================================================================================
来源：http://hz.sysykeji.top/gtwvrmnscs.html

[R01] shebang 与严格模式
来源：http://hz.tian-w.cn/gtbptsxzoz.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gtpgdxqnbs.html

set -euo pipefail
来源：http://hz.yueranfly.top/gtvqkpcytm.html

[R02] 变量赋值与使用
来源：http://hz.ppjwa.cn/gtxuwywymh.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtcablixzw.html

[R03] 只读变量
来源：http://hz.cqqwz.cn/gtprxurczz.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtfgjkrwot.html

[R04] 位置参数
来源：http://hz.yvedp.cn/gtvrfijtrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenzaomai.com/gttqfcxune.html

[R05] 参数默认值
来源：http://hz.jlsjyb.cn/gtqynedmmp.html

name="${1:-default}"
来源：http://hz.jqgfzy.top/gtslwtqwgr.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gtdrntwbjh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtiwmfnamr.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtrmqlqriz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtylexkulb.html

[R08] 数值比较
来源：http://hz.shanyushiyangkeji.top/gtdbeesvvy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangtech.top/gtnddcpqvl.html

[R09] 字符串比较
来源：http://hz.shanyushiyangtech.top/gteupqaqtk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258.top/gtocsthcup.html

[R10] 正则匹配
来源：http://hz.zhoulong.xyz/gtdlugsspu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtlfcndgai.html

[R11] case 多分支
来源：http://hz.52xcode.cn/gtlauxempq.html

case "$1" in
来源：http://hz.jiagoushi.top/gtiwtfqefq.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtlppnnffz.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtvkdpblip.html

*)     echo "未知命令" ;;
来源：http://hz.jqgfzy.top/gtonqvdrzb.html

esac
来源：http://hz.yueranfly.top/gtxlpetqle.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtobqsqkjo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cdnleiting.top/gtemngkhna.html

[R13] for 计数循环
来源：http://hz.yj202588.top/gtgoxlctbj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cheryme.top/gtldiebyri.html

[R14] C 风格 for
来源：http://hz.0kj1m.cn/gtdlfafvmu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gthhjpnejj.html

[R15] while 逐行读文件
来源：http://hz.mhx1999.top/gtjovjhxtl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtlgecjdnz.html

[R16] until 等待条件
来源：http://hz.0kj1m.cn/gthxcuwkvw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yonumen.top/gtfpstdcpb.html

[R17] 数组定义与取值
来源：http://hz.mhx1999.top/gtwjuxrmok.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuetiantiany.cn/gtdmqmvlrx.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtazjcfzai.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ppjwa.cn/gtgmgurznq.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtyufjikzo.html

echo "${#arr[@]}"
来源：http://hz.yuxming.cn/gttylfngki.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gthlluvgld.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.birdmap.top/gtbfdkfrzc.html

[R21] 字符串长度
来源：http://hz.sxryk.cn/gtacjzmcng.html

echo "${#s}"
来源：http://hz.hammf.cn/gtubmqkrpw.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtftcyundz.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gtvwfuphrh.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtnaujomyg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gtfeluygvv.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtfstaqfku.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtfwpktrve.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtoxmenjzj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtwdhthzxs.html

[R26] 命令替换
来源：http://hz.mhx1999.top/gtnjklxtqq.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgfzy.top/gtdhjkxqyf.html

[R27] 算术展开
来源：http://hz.hnxiangtu.top/gtiirzjcvc.html

echo $((1 + 2 * 3))
来源：http://hz.shzxlz.cn/gtgqirodoy.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtvosjctzk.html

echo "scale=2; 10/3" | bc
来源：http://hz.guannengcc.top/gtejpjcpzy.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtfwlotttu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xingfuxueyuan.xyz/gtxtdwgypt.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtbwbmvfjt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtlypudljz.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtukieodgs.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtaghkifdk.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtnsnhvbwd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gaohongyu789.top/gtytrbsgqw.html

[R33] 捕获错误并提示行号
来源：http://hz.hammf.cn/gtjkigzami.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtaasmrahj.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtndtrfmaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtcirozbpe.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtsukfkyzh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tianlin.xyz/gtfbznxflu.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtsrxxzmql.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dashuyun.cn/gtlzqowqyq.html

[R37] 把输出赋给变量
来源：http://hz.feifeiyinyue.top/gtgtenhpqn.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gtqbqrlbhf.html

[R38] 管道串联
来源：http://hz.svipenyu.cn/gtpdajzmho.html

cat a.txt | grep -i error | wc -l
来源：http://hz.snrcjt.cn/gttpnstroy.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtsejxjncl.html

cmd > out.log 2>&1
来源：http://hz.nwbrower.top/gtkcoaoctg.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtotquxlnn.html

echo "log" >> out.log
来源：http://hz.chenlongwang.top/gtufuecerr.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtzbtsynii.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtbgmsqxeh.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtcsgxexhg.html

wc -l < a.txt
来源：http://hz.hfpthk.cn/gtenqtotku.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtgalntkbl.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangtech.top/gtrryvuelr.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtzjeikuyn.html

find . -mtime -7 -type f
来源：http://hz.jyoumei.cn/gtkjveephz.html

[R45] 批量删除
来源：http://hz.ivvv.top/gtrarhpfux.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gtadbzebgs.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtkfsoqeiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jianghu66.top/gttphxzkyu.html

[R47] sed 单行替换
来源：http://hz.hongshengwenyu.top/gtkbpntxti.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gtsinwxkxj.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gtuadnfymp.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gtjthpskwq.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gtnfxtwpli.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtnwqgilfj.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtzzqwejcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pengpengdd.cyou/gtrnbahxkc.html

[R51] 排序去重取前几
来源：http://hz.dashuyun.cn/gtyudywzeq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yvedp.cn/gttyehjcid.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gtyegwisgr.html

wc -l a.txt
来源：http://hz.nwbrower.top/gtbghprhmw.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtppfahytt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.redwolf501.top/gtbcxegxnt.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gtqgscenag.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtpbgfswvg.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangtech.top/gtkxznmyur.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtvsqeioff.html

[R56] 远程拷贝
来源：http://hz.aizwys.cn/gttjqqurjs.html

scp file user@host:/path/
来源：http://hz.gaohongyu789.top/gtefwqytso.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtmnsowfgx.html

ssh user@host 'uptime'
来源：http://hz.tanke756.top/gtzfgphkdx.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtryvwtssz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xinyue.icu/gtywemvxch.html

[R59] 发 POST JSON
来源：http://hz.vqdsnc.cn/gtmsetyyvb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtyyqfvcic.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258.top/gtztshrucp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtrjfpggtr.html

[R61] 磁盘占用
来源：http://hz.sysykeji.top/gtyqemdjvr.html

df -h;  du -sh *
来源：http://hz.tian-w.cn/gthvfkykjm.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtieybxjyq.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtyyxqyihc.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtphkmndjk.html

free -h;  ps aux | grep nginx
来源：http://hz.hywenlv.cn/gtipnksuwc.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gttymajclj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nanxinkj.top/gtafaonawm.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gthfovlznb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtmxsyfjov.html

[R66] 定时任务
来源：http://hz.nanxuanxn.top/gtcqkzuydn.html

crontab -e;  crontab -l
来源：http://hz.9152youxi.cn/gtxgwwhncd.html

[R67] 生成随机十六进制串
来源：http://hz.hfpthk.cn/gtdmpuiess.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gtectuzxvs.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtebrszguj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gtfacuymtu.html

[R69] 生成随机密码
来源：http://hz.c1oappe.top/gtgunmomsi.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtizyixssz.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gtufzxbsyd.html

date +%s;  date -d @1700000000
来源：http://hz.9152youxi.cn/gtnhqlhqzi.html

[R71] 日期格式化
来源：http://hz.jqgfzy.top/gtlgvtwryi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtifmpreqc.html

[R72] 等待端口就绪
来源：http://hz.jqgufenzy.top/gtygylgcsx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258.top/gtqbsogyjh.html

[R73] 分割大日志
来源：http://hz.pycfn.com/gtnxdqryua.html

split -l 1000 big.log part_
来源：http://hz.tian-w.cn/gtzuzqhzlz.html

[R74] 批量重命名
来源：http://hz.zhengqikj.top/gtzzvchpyv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yongpay.top/gtlxvuqdnk.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtfwudrmnu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.birdmap.top/gtfronppur.html

[R76] 使用临时文件
来源：http://hz.redwolf501.top/gtzjiufgtm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtfuaspjec.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gtagmondcy.html

read -rp "请输入: " ans
来源：http://hz.52xcode.cn/gtkaxkppzd.html

[R78] 交互式菜单
来源：http://hz.ydjk.org.cn/gtdividywo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.vqdsnc.cn/gtqyflmlgh.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gtszrjirtf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuanzx.com/gtmoheshmp.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtkcwdofti.html

time ./run.sh
来源：http://hz.cucudq.cn/gtfahcckwd.html

================================================================================
来源：http://hz.dianchejie.cn/gtjwxysiwm.html

S. C / C++ 专题
来源：http://hz.daria6918.cn/gtauusybmk.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxgblfifb.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtkycmfhrz.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtvqkevpwe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gteziffkgl.html

[S02] C：变量与格式化输出
来源：http://hz.ywan-chungtsiang.top/gtcbdnypmg.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gtiiiwxpze.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gttwiqzrfm.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gtxtlcuven.html

[S04] C：字符串复制
来源：http://hz.hywenlv.cn/gtlmbfczye.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtpipueyff.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtkofcexux.html

strlen(s)
来源：http://hz.shzxlz.cn/gtnteowcqu.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtemazrctn.html

strcmp(a, b) == 0
来源：http://hz.316326.xyz/gtcrdixihe.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangtech.top/gtrabvlxon.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtssulzlmz.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtatokfvpq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.smart0.xyz/gtceoxbkye.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtrnxfuzes.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gtdltnbgal.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gttcrbbaef.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtdsgexqct.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtiypmedgd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gtcruvodqx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hywenlv.cn/gtrlzndouo.html

fclose(f);
来源：http://hz.hammf.cn/gtgosygmtm.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtuzpzrhbv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gthfczlbsu.html

[S13] C：宏定义
来源：http://hz.cheryme.top/gtebrpocaq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtvdcxnnwk.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtircviaut.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gtufynzlif.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gtsotipguq.html

(double) a / b
来源：http://hz.sufxvd.cn/gtohbnamoj.html

[S16] C：位操作置位
来源：http://hz.aibaodan.cn/gtyiydabzn.html

x |= (1 << 3);
来源：http://hz.chenzaomai.com/gtyvxvglsu.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtxtwjsjue.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenjidiqi.icu/gtrwlzzwgy.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtwrgmgefu.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtlfekdfts.html

[S19] C：快速排序
来源：http://hz.ivvv.top/gtfoatifac.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtwhupsiys.html

[S20] C：二分查找
来源：http://hz.cucudq.cn/gtlxpapxve.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtgsdgmxfu.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtpxzzszxa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtzhcyrtjc.html

[S22] C：字符串转数字
来源：http://hz.xingfuxueyuan.xyz/gttnlmxofm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.andypj.xyz/gtrzokmbwo.html

[S23] C：随机数
来源：http://hz.hongshengwenyu.top/gtuutydwjo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydzc1.top/gtijyogtrd.html

[S24] C：获取本地时间
来源：http://hz.52xcode.cn/gtvltcfvnx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangkeji.top/gthbzdkohm.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtjpxbtfpd.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtnfqipttr.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtmnhxloam.html

memset(a, 0, sizeof a);
来源：http://hz.hongshengwenyu.top/gtxlfhiwde.html

[S27] C：定义常量
来源：http://hz.chenzaomai.com/gtahizrbie.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtbgjpogft.html

[S28] C：静态变量
来源：http://hz.mhx1999.top/gtofahkzif.html


<!-- 参考信息 -->